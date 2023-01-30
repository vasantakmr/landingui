<svelte:options tag="typewriter-js" />

<script lang="ts">
    import { onMount } from "svelte";

    export let textdata;
    let elem;

    var TxtType = function(el, toRotate, period) {
        this.toRotate = toRotate;
        this.el = el;
        this.loopNum = 0;
        this.period = parseInt(period, 10) || 2000;
        this.txt = '';
        this.tick();
        this.isDeleting = false;
    };

    TxtType.prototype.tick = function() {
        var i = this.loopNum % this.toRotate.length;
        var fullTxt = this.toRotate[i];

        if (this.isDeleting) {
        this.txt = fullTxt.substring(0, this.txt.length - 1);
        } else {
        this.txt = fullTxt.substring(0, this.txt.length + 1);
        }

        this.el.innerHTML = '<span class="wrap">'+this.txt+'</span>';

        var that = this;
        var delta = 200 - Math.random() * 100;

        if (this.isDeleting) { delta /= 2; }

        if (!this.isDeleting && this.txt === fullTxt) {
        delta = this.period;
        this.isDeleting = true;
        } else if (this.isDeleting && this.txt === '') {
        this.isDeleting = false;
        this.loopNum++;
        delta = 500;
        }

        setTimeout(function() {
        that.tick();
        }, delta);
    };

    function typewrite() {
        var toRotate = textdata;
        var period = elem.getAttribute('data-period');
        if (toRotate) {
            new TxtType(elem, JSON.parse(toRotate), period);
        }
        // INJECT CSS
        var css = document.createElement("style");
        css.type = "text/css";
        css.innerHTML = ".typewrite > .wrap { border-right: 0.08em solid #fff}";
        document.body.appendChild(css);
    };

    onMount(async () => {
		typewrite();
	});
   

</script>

<a href="" bind:this={elem} class="typewrite" data-period="2000" data-type={textdata}>
    <span class="wrap"></span>
</a>
  
<style lang="scss">

    .typewrite {
        @apply text-black bg-yellow-400
    }

</style>