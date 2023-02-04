<svelte:options tag="carousel-ui" />

<script lang="ts">
    import { onMount } from "svelte";

    let keyRoot;
    let cards;    

    onMount(async () => {
		console.log(keyRoot)
        cards = keyRoot.querySelectorAll('.card');
        let activeCard = cards[0];

        cards.forEach((card) => {
            card.addEventListener('click', () => {
                activeCard.classList.remove('active');
                activeCard = card;
                activeCard.classList.add('active');
                console.log("hellowrld");
            });
        });
	});

</script>


<div bind:this={keyRoot} class="outerMost">
    <div class="outerInn">
      <div class="active card inner0">
        <div class="inner1 background red"></div>
        <div class="inner2 shadow"></div>
        <div class="inner3 label">
          <div class="inner4"><i class="fas fa-walking"></i></div>
          <div class="inner5 content">
            <div class="inner6">Lights</div>
            <div class="inner7">Chase your dreams</div>
          </div>
        </div>
      </div>
      <div class="card inner0">
        <div class="inner1 background yellow"></div>
        <div class="inner2"></div>
        <div class="inner3 label">
          <div class="inner4 text-yellow-500"><i class="fas fa-apple-alt"></i></div>
          <div class="inner5 content">
            <div class="inner6">Construction</div>
            <div class="inner7">Build the extraordinary</div>
          </div>
        </div>
      </div>
      <div class="card inner0">
        <div class="inner1 background green"></div>
        <div class="inner2"></div>
        <div class="inner3 label">
          <div class="inner4 text-green-500"><i class="fas fa-tree"></i></div>
          <div class="inner5 content">
            <div class="inner6">Landscape</div>
            <div class="inner7">Explore the surroundings</div>
          </div>
        </div>
      </div>
      <div class="card inner0">
        <div class="inner1 background blue"></div>
        <div class="inner2"></div>
        <div class="inner3 label">
          <div class="inner4 text-blue-500"><i class="fas fa-tint"></i></div>
          <div class="inner5 content">
            <div class="inner6">Pools</div>
            <div class="inner7">Soak in tranquility</div>
          </div>
        </div>
      </div>
      <div class="card inner0">
        <div class="inner1 background purple"></div>
        <div class="inner2"></div>
        <div class="inner3 label">
          <div class="inner4 text-purple-500"><i class="fas fa-palette"></i></div>
          <div class="inner5 content">
            <div class="inner6">Reflect</div>
            <div class="inner7">Harness your potential</div>
          </div>
        </div>
      </div>
    </div>
</div>



<style lang="scss">

    .red {
        @apply bg-red-500 bg-red-img;
    }

    .yellow {
        @apply bg-yellow-500 bg-yellow-img;
    }

    .green {
        @apply bg-green-500 bg-green-img;
    }

    .blue {
        @apply bg-blue-500 bg-blue-img;
    }

    .purple {
        @apply bg-purple-500 bg-purple-img
    }
    .outerMost {
        @apply antialiased flex font-sans items-center justify-center px-6;
    }

    .outerInn {
        @apply flex h-72 items-stretch max-w-2xl overflow-hidden w-full;
    }

    .inner0 {
        @apply card cursor-pointer duration-700 ease-in-out flex-grow m-2 min-w-14 overflow-hidden relative rounded-3xl transition-all;
    }

    .inner1 {
        @apply absolute background bg-center bg-cover bg-no-repeat duration-700 ease-in-out inset-0 scale-105 transition-all z-10;
    }

    .inner2 {
        @apply absolute bg-gradient-to-b bottom-0 duration-700 ease-in-out from-transparent h-1/2 inset-x-0 opacity-0 shadow to-black transform transition-all translate-y-1/2 z-20;
    }

    .inner3 {
        @apply absolute bottom-0 duration-700 ease-in-out flex label left-0 mb-3 ml-2 transition-all z-30;
    }

    .inner4 {
        @apply bg-black flex h-10 items-center justify-center mr-3 rounded-full text-red-500 w-10;
    }

    .inner5 {
        @apply flex flex-col justify-center leading-tight text-white whitespace-pre;
    }

    .inner6 {
        @apply ease-in-out font-bold duration-700 opacity-0 relative transform transition-all translate-x-8;
    }

    .inner7 {
        @apply delay-100 duration-700 ease-in-out opacity-0 relative transform transition-all translate-x-8;
    }

    .card.active {
        flex-grow: 10;
        max-width: 100%;	
    }

    .background {
        transform: scale(1.25, 1.25);
    }

    .label {
        transform: translateX(0.5rem);
    }

    .content > * {
        opacity: 1;
        transform: translateX(0);
    }

    .shadow {
        opacity: 0.75;
        transform: translateY(0);
    }
</style>