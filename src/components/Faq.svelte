<script>
  import faqList from '../data/faqList';
</script>


<div data-aos="fade-up" class="bg-dark pt-8 p-4 sm:p-6 lg:max-w-screen-md md:max-w-screen-md w-full flex-col flex items-center text-gray-500  rounded-lg border border-gray-200 dark:border-gray-700 shadow-md flex  flex-col">
  <h3 class="mb-2 text-6xl font-magic text-center tracking-tight text-red-500">
    Odpowiedzi na pytania
  </h3> 

  <ol class="w-full"> 
  {#each faqList as faq}
  <li style="" class="rounded-lg m-1 hover:bg-white">
    <p on:click={() => faq.showText = !faq.showText} class="p-5 font-medium text-gray-900" id="accordion-collapse-heading-1">
      {faq.title} ?
    </p>
    {#if faq.showText}
    <div id="accordion-collapse-body-1" class="p-5 font-light hover:bg-white" aria-labelledby="accordion-collapse-heading-1">
        {#each faq.desctiption as desctiption}
          <p class="mb-2 text-gray-900 ">{desctiption}</p>
        {/each}
    </div>
    {/if}
  </li>
  {/each}
  </ol>
</div>
