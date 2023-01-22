<script>
    import workshopsList from '../data/workshopsList';
</script>


    <ol>
        {#each workshopsList as workshop}
        <li 
        data-aos="zoom-in"
        class="p-4 sm:p-6 m-2 rounded-lg  hover:bg-dark">
            <h3 class="mb-2 text-2xl font-bold tracking-tight text-white">
                <span class="mb-4 mt-4 text-2xl font-bold text-gray-900">#{workshop.id + 1}</span> {workshop.title}
            </h3> 
            <p class="mt-2 mb-1  text-gray-600 font-normal leading-tight">
                {workshop.goal}
            </p>
            <!-- text-sm  -->
            <!-- {#each workshop.descr as descr}
              <p class="mb-1 font-normal text-gray-600 leading-tight">
                  {descr}.
              </p>
            {/each} -->
            <p class="mb-2 mt-2 text-1xl font-normal text-gray-600">🏠 {workshop.addres}</p>
            <!-- <span>{workshop.date}</span>
            <span>{workshop.maxVisitors}</span>
            <span>{workshop.startTime}</span>
            <span>{workshop.endTime}</span> -->

            <div class="m-1 flex flex-row justify-center p-2 rounded-lg">
              <span class="text-2xl font-bold text-gray-800 ">{workshop.duration} min</span>
              <span class="text-2xl font-bold text-gray-800 mr-2 ml-2"> / </span>
              <span class="text-2xl font-bold text-gray-800 ">{workshop.maxVisitors} miejsc</span>
            </div>
            <div class="m-1 flex flex-row justify-center p-2 rounded-lg">
              <span class="text-2xl font-bold text-gray-800 ">{workshop.startTime}</span>
              <span class="text-2xl font-bold text-gray-800 mr-2 ml-2"> - </span>
              <span class="text-2xl font-bold text-gray-800 ">{workshop.endTime}</span>
            </div>

            <div class="mt-4 flex justify-between items-center p-2 rounded-lg">
                <span class="text-3xl font-bold text-gray-800 ">{workshop.date}</span>
                <button type="button" class="bg-gray-900 text-center font-medium focus:ring-4 focus:outline-none inline-flex items-center justify-center px-6 py-3.5 text-base text-white hover:bg-dark focus:ring-white-300 rounded-lg">
                    More
                </button>
            </div>
        </li>   
        {/each} 
    </ol>


<style>
ol {
  margin: 0;
  list-style: none;
  padding: 0;
  --hue: 1;
  --unit: 1rem;
}

li {
  --height: 7rem;
  position: relative;
  display: block;
  background-color: hsl(calc(var(--hue)*360/20),90%,65%);
  border-color: hsl(calc(var(--hue)*360/20),90%,65%);
  padding: 1rem;
  margin: 2rem 0;
}
li::before {
  content: "";
  background-color: inherit;
  position: absolute;
  display: block;
  width: var(--unit);
  height: var(--unit);
  top: 100%;
  left: calc(50% - (var(--unit)/2));
}
li::after {
  content: "";
  position: absolute;
  display: block;
  top: calc(100% + var(--unit));
  left: calc(50% - (var(--unit)));
  border: var(--unit) solid transparent;
  border-top-color: inherit;
}
li:last-child::before,
li:last-child::after {
  content: none;
}

@media (min-width: 550px) and (max-width: 899px){
  li {
    margin: 1rem;
    width: calc(50% - 4rem);
    float: left;
    min-height: var(--height);
  }
  li:nth-child(4n+3),
  li:nth-child(4n+4) {
    float: right;
  }
  li:nth-child(4n+1)::before {
    top: calc(var(--height)/2 + var(--unit)/2);
    left: 100%;
  }
  li:nth-child(4n+1)::after {
    top: calc(var(--height)/2);
    left: calc(100% + (var(--unit)));
    border: var(--unit) solid transparent;
    border-left-color: inherit;
  }
  li:nth-child(4n+3)::before {
    top: calc(var(--height)/2 + var(--unit)/2);
    left: -1rem;
  }
  li:nth-child(4n+3)::after {
    top: calc(var(--height)/2);
    left: -3rem;
    border: var(--unit) solid transparent;
    border-right-color: inherit;
  }
}
@media (min-width: 900px) and (max-width: 1199px){
  li {
    margin: 1rem;
    width: calc(33.33% - 4rem);
    float: left;
    min-height: 7rem;
  }
  li:nth-child(6n+4),
  li:nth-child(6n+5),
  li:nth-child(6n+6) {
    float: right;
  }
  li:nth-child(6n+1)::before,
  li:nth-child(6n+2)::before {
    top: calc(var(--height)/2 + var(--unit)/2);
    left: 100%;
  }
  li:nth-child(6n+1)::after,
  li:nth-child(6n+2)::after {
    top: 3.5rem;
    left: calc(100% + (var(--unit)));
    border: var(--unit) solid transparent;
    border-left-color: inherit;
  }
  li:nth-child(6n+4)::before,
  li:nth-child(6n+5)::before{
    top: calc(var(--height)/2 + var(--unit)/2);
    left: -1rem;
  }
  li:nth-child(6n+4)::after,
  li:nth-child(6n+5)::after{
    top: calc(var(--height)/2);
    left: -3rem;
    border: var(--unit) solid transparent;
    border-right-color: inherit;
  }
}
@media (min-width: 1200px){
  ol {
    max-width: 1600px;
    margin: 0 auto;
  }
  li {
    margin: 1rem;
    width: calc(25% - 3rem);
    float: left;
    min-height: 7rem;
  }
  li:nth-child(8n+5),
  li:nth-child(8n+6),
  li:nth-child(8n+7),
  li:nth-child(8n+8){
    float: right;
  }
  li:nth-child(8n+1)::before,
  li:nth-child(8n+2)::before,
  li:nth-child(8n+3)::before{
    top: calc(var(--height)/2 + var(--unit)/2);
    left: 100%;
  }
  li:nth-child(8n+1)::after,
  li:nth-child(8n+2)::after,
  li:nth-child(8n+3)::after{
    top: calc(var(--height)/2);
    left: calc(100% + (var(--unit)));
    border: var(--unit) solid transparent;
    border-left-color: inherit;
  }
  li:nth-child(8n+5)::before,
  li:nth-child(8n+6)::before,
  li:nth-child(8n+7)::before {
    top: calc(var(--height)/2 + var(--unit)/2);
    left: -1rem;
  }
  li:nth-child(8n+5)::after,
  li:nth-child(8n+6)::after,
  li:nth-child(8n+7)::after {
    top: calc(var(--height)/2);
    left: -3rem;
    border: var(--unit) solid transparent;
    border-right-color: inherit;
  }
}
</style>