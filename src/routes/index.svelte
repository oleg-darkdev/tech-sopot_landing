<script>
	import Timeline from '../components/Timeline.svelte';
	import Faq from '../components/Faq.svelte';
</script>

<svelte:head>
	<title>Najlepsza praca "Henry Forda"</title>
</svelte:head>


<section class="w-full pt-4 pb-6">
	<div class="bg-blue-500 max-w-screen-md text-gray-500  rounded-lg border border-gray-200 dark:border-gray-700 shadow-md flex  flex-col">
	<img class="rounded-t-lg" src="/banner.png" alt=""> 
	<div class="p-4 sm:p-6 flex flex-col items-center">
		<h2 class="mb-2 text-6xl font-magic tracking-tight text-dark">
			O projekcie
		</h2> 
		<!-- <p class="w-12/12 lg:w-9/12 md:w-10/12 text-center font-normal text-gray-900 mb-4 leading-tight">
			Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
		</p> -->
		<h3 class="mb-2 text-2xl font-bold tracking-tight text-dark">
			Cele projektu
		</h3> 
		<ol class="mb-2  items-center text-white max-w-md list-disc list-inside space-y-1">
			<li data-aos="fade-up" class="text-c font-semibold rounded-md p-2 text-dark hover:bg-white">
				ukazanie różnej specyfiki i problemów różnych zawodów
			</li>
			<li data-aos="fade-up" class="text-c font-semibold rounded-md p-2 text-dark  hover:bg-white">
				wprowadzenie młodych ludzi w świat IT, omoc w rozpoczęciu pracy w zawodzie IT
			</li>
			<li data-aos="fade-up" class="text-c font-semibold rounded-md p-2 text-dark  hover:bg-white">
				pokazanie, że nauka każdego zawodu jest możliwa dzięki zaangażowaniu w wolontariacie
			</li>
			<li data-aos="fade-up" class="text-c font-semibold rounded-md p-2 text-dark  hover:bg-white">
				rozwijanie logicznego i abstrakcyjnego myślenia poprzez szachy i programowanie
			</li>
		</ol>

		<div class="flex flex-row mb-4 flex-wrap justify-center">
			<div data-aos="fade-right" class="m-1 bg-orange-300 text-gray-500  rounded-lg  shadow-md flex max-w-sm flex-col hover:bg-gray-100 dark:hover:bg-gray-700 p-4 sm:p-6">
				<h4 class="mb-2  text-2xl font-bold tracking-tight text-gray-900">
					Terminy realizacji
				</h4> 
				<p class="font-normal text-gray-700  leading-tight">
					17.01.2023 - 30.08.2023
				</p>
			</div>

			<div data-aos="fade-left" class="m-1 bg-green-300 text-gray-500  rounded-lg  shadow-md flex max-w-sm flex-col hover:bg-gray-100 dark:hover:bg-gray-700 p-4 sm:p-6">
				<h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900">
					Grupa docelowa
				</h5> 
				<p class="font-normal text-gray-700  leading-tight">
					Młodzież w wieku 16-17 lat
				</p>
			</div>
		</div>

		<span class="text-center  mb-2 mt-6 font-normal text-gray-900  leading-tight">
			Projekt jest dostępny w mediach
		</span>
        <div class="w-full  flex flex-wrap justify-center content-center flex-row mb-6 rounded-xl">
          <a href=''>
            <img src="social/facebook.svg" class="w-20 h-20 m-1 rounded-lg border-2 border-dark bg-blue-600   hover:bg-white hover:border-white  social-hover" alt="">

          </a>
          <a href=''>
            <img src="social/github.svg" class="w-20 h-20 m-1 rounded-lg border-2 border-dark bg-blue-600 hover:bg-white hover:border-white social-hover" alt="">

          </a>

        </div>
	</div>
	</div>
</section>


<section class="w-full pt-12 pb-12 flex flex-col items-center bg-dark">
<div class="p-10 bg-white md:w-11/12 lg:w-11/12 w-12/12 border-2 border-dark  rounded-lg border  shadow-md flex  flex-col items-center">

	<h2 class="mb-2 text-6xl font-magic tracking-tight text-dark">
		Plan lekcji
	</h2> 
	<Timeline />
</div>
</section>

<section class="w-full flex flex-col items-center">
		<Faq />
</section>

<style>

</style>