<svelte:options tag="landing-page-animation" />

<script lang="ts">
	let selected: string;

	function lightToggle() {
		if(selected === "on") {
			selected = "off"
		} else {
			selected = "on"
		}
	}
</script>

<div>
	<div class="luminaire" on:click={lightToggle} class:on={selected === "on"}></div>
	<div class="luminaire" on:click={lightToggle} class:on={selected === "on"}></div>	
</div>
<div>
	<div class="luminaire" on:click={lightToggle} class:on={selected === "on"}></div>
	<div class="luminaire" on:click={lightToggle} class:on={selected === "on"}></div>	
</div>

<style lang="scss">

	
.luminaire {
    position: relative;
    display: inline-block;
    width: 30px;
    height: 30px;
    margin: 60px;
    border-radius: 50%;
    background-color: #000;
    box-shadow: 0 0 40px 20px #fff, 0 0 100px 50px #0ff;
    transition: box-shadow 4s ease-out;
    animation: spin 16s linear infinite;
  }
  @keyframes spin {
    100% {
      transform: rotate(360deg);
    }
  }
  
  .luminaire:hover {
    cursor: pointer;
  }
  
  .luminaire::before, .luminaire::after {
    content: '';
    display: block;
    position: absolute;
    top: calc(50% - 10px);
    left: calc(50% - 10px);
    width: 20px;
    height: 20px;
    border-radius: 50%;
    background-color: #fff;
    box-shadow: 0 0 40px 20px #fff, 0 0 100px 50px #ff0;
    opacity: 0;
    transition: opacity 8s, transform 8s;
  }
  
  .on {
    background-color: #fff;
    box-shadow: 0 0 80px 40px #fff, 0 0 200px 100px #f0f;
  }
  
  .on::before {
    transform: translateX(-100px);
    opacity: 1;
  }
  
  .on::after {
    transform: translateX(100px);
    opacity: 1;
  }


  
</style>