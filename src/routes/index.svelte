<script>
	import Timeline from '../components/Timeline.svelte';
	import Faq from '../components/Faq.svelte';
</script>

<svelte:head>
	<title>Najlepsza praca "Henry Forda"</title>
</svelte:head>


<section class="w-full pt-12 pb-6">
	<div class="bg-blue-500 max-w-screen-md text-gray-500  rounded-lg border border-gray-200 dark:border-gray-700 shadow-md flex  flex-col">
	<img class="rounded-t-lg" src="/banner.png" alt=""> 
	<div class="p-4 sm:p-6 flex flex-col items-center">
		<h2 class="mb-2 text-6xl font-magic tracking-tight text-dark">
			O projekcie
		</h2> 
		<div class="flex flex-row mb-4 flex-wrap justify-center">
			<div data-aos="fade-right" class="m-1 bg-orange-300 text-gray-500  rounded-lg  shadow-md flex max-w-sm flex-col hover:bg-gray-100 dark:hover:bg-gray-700 p-4 sm:p-6">
				<h3 class="mb-2  text-2xl font-bold tracking-tight text-gray-900">
					Terminy realizacji
				</h3> 
				<p class="font-normal text-gray-700  leading-tight">
					17.01.2023 - 30.08.2023
				</p>
			</div>

			<div data-aos="fade-left" class="m-1 bg-green-300 text-gray-500  rounded-lg  shadow-md flex max-w-sm flex-col hover:bg-gray-100 dark:hover:bg-gray-700 p-4 sm:p-6">
				<h3 class="mb-2 text-2xl font-bold tracking-tight text-gray-900">
					Grupa docelowa
				</h3> 
				<p class="font-normal text-gray-700  leading-tight">
					Młodzież w wieku 16-17 lat
				</p>
			</div>
		</div>
		<p class="w-12/12 lg:w-10/12 md:w-10/12 font-normal text-gray-900 mb-1 leading-tight">
			Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
		</p>
		<p class="w-12/12 lg:w-10/12 md:w-10/12 mb-4 font-normal text-gray-900  leading-tight">
			Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
		</p>

		<h4 class="mb-2 text-2xl font-bold tracking-tight text-dark">
			Cele projektu
		</h4> 
		<ol class="mb-4  items-center text-white max-w-md list-disc list-inside space-y-1">
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

		
		
		<div class="flex justify-end w-full">
			<button type="button" class="max-w-sm text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-5 py-2.5 text-sm text-dark bg-white hover:bg-gray-600 rounded-lg">
				Zarejestruj się na szkolenie 
			<svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 ml-2">
				<path stroke-linecap="round" stroke-linejoin="round" d="M13.5 4.5L21 12m0 0l-7.5 7.5M21 12H3">
				</path>
			</svg>
			</button>
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

<section class="w-full p-12 flex flex-col items-center">
	<div class="lg:w-6/12 md:w-6/12 w-11/12 ">
		<Faq />
	</div>
</section>

<style>

</style>