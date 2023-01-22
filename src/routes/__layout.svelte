<script>
    import '../app.css';  
    import 'aos/dist/aos.css';
    import AOS from 'aos';
    import { onMount } from 'svelte';
    onMount(() => {
      AOS.init();
    });

    import Footer from '../layout/Footer.svelte';
</script>


<slot />

<Footer />

<style>
 :global(.font-magic) {
          font-family: 'Magic';
            line-height: 1.2;
  }

  	:global(ol) {
		--hue: 1;
	}
	:global(li) {
		background-color: hsl(calc(var(--hue)*360/20),90%,65%);
		border-color: hsl(calc(var(--hue)*360/20),90%,65%);
	}

  :global(li > div) {
		background-color: hsl(calc(var(--hue)*360/20),80%,55%);
		border-color: hsl(calc(var(--hue)*360/20),90%,65%);
	}
	:global(li:nth-child(20n+1)){
	--hue: 1;
	}
	:global(li:nth-child(20n+2)){
	--hue: 2;
	}
	:global(li:nth-child(20n+3)){
	--hue: 3;
	}
	:global(li:nth-child(20n+4)){
	--hue: 4;
	}
	:global(li:nth-child(20n+5)){
	--hue: 5;
	}
	:global(li:nth-child(20n+6)){
	--hue: 6;
	}
  
:global(li:nth-child(20n+7)){
  --hue: 7;
}
:global(li:nth-child(20n+8)){
  --hue: 8;
}
:global(li:nth-child(20n+9)){
  --hue: 9;
}
:global(li:nth-child(20n+10)){
  --hue: 10;
}
:global(li:nth-child(20n+11)){
  --hue: 11;
}
:global(li:nth-child(20n+12)){
  --hue: 12;
}
:global(li:nth-child(20n+13)){
  --hue: 13;
}
:global(li:nth-child(20n+14)){
  --hue: 14;
}
:global(li:nth-child(20n+15)){
  --hue: 15;
}
:global(li:nth-child(20n+16)){
  --hue: 16;
}
:global(li:nth-child(20n+17)){
  --hue: 17;
}
:global(li:nth-child(20n+18)){
  --hue: 18;
}
:global(li:nth-child(20n+19)){
  --hue: 19;
}
:global(li:nth-child(20n+20)){
  --hue: 20;
}
:global(li:nth-child(20n+21)){
  --hue: 21;
}
:global(li:nth-child(20n+22)){
  --hue: 22;
}
:global(li:nth-child(20n+23)){
  --hue: 23;
}
:global(li:nth-child(20n+24)){
  --hue: 24;
}
@font-face {
    font-family: 'Magic';
    font-style: normal;
    font-weight: 500;
    
    src: local(''),
        /* Super Modern Browsers */ url('/fonts/magic.woff') format('woff'),
        /* Modern Browsers */ url('/fonts/magic.ttf') format('truetype'),
        /* Safari, Android, iOS */ url('/fonts/magic.svg') format('svg'); /* Legacy iOS */
}

	:global(section) {
		margin-bottom: 30px;
	}
	:global(.justify-center, section)  {
        display: flex;
        justify-content: center;
    }
    :global(.row) {
        display: flex;
        flex-direction: row;
    }
	:global(column) {
        display: flex;
		flex-direction: column;
	}

    :global(.bg) {
        background-repeat: no-repeat;
        background-position: center;
    }

	:global(body, html) {
		height: 100%;
		margin: 0;
		padding: 0;
	}
</style>
