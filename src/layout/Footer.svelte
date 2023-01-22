<script>
    import partnersList from '../data/partnersList';
</script>


<footer class="w-full flex justify-center">

   
  <div class="sm:flex sm:items-center sm:justify-between w-8/12 rounded-lg p-4 bg-blue-500  shadow md:px-6 md:py-8 ">
        <span class="mb-2 text-1xl tracking-tight text-white" style="max-width: 200px;">
			Projekt został zrealizowany przy wsparciu następujących organizacji
		</span> 
   		<div class="p-0 m-0 flex flex-wrap flex-row justify-center w-full">
            {#each partnersList as partner}
                <div
                    class="m-1 partners-logos rounded-lg border border-gray-300 "
                    style="background-image: url({partner.logoImg});"
                />
            {/each}
        </div>
   
  </div> 
</footer>
	

<style>
    .partners-logos {
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
		height: 60px;
		width: 140px;
	}

    .partners-logos-wrap {
		display: flex;
		flex-direction: row;
        justify-content: center;
		/*  */

		/* max-width: 50vw; */
		width: auto;
		height: auto;
		flex-wrap: wrap;
	}
</style>
