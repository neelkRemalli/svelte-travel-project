<script>
    import HeaderSection from './HeaderSection.svelte'
    import {fly} from 'svelte/transition'
    import Button from './Button.svelte'
    const ListTravel = [
        {name: 'Travel Trends'},
        {name: 'Packing Tips'},
        {name: 'Responsible Travel'},
        {name: 'Mobile Apps'},
    ]
    let y;
</script>
<svelte:window  bind:scrollY={y}/>
<div class='mt-20 px-4'>
    <HeaderSection title='Travel Tips' />
    <div class='grid sm:grid-cols-2 grid-cols-1'>
        <div class='mx-16 xl:mx-0'>
         <ul class='flex flex-col justify-center'>
       {#each ListTravel as item, i}
       {#if y >= 1800  }
       <li class='md:text-xl text-gray-800 uppercase font-bold mb-3' transition:fly={{x:-200, delay: 300, duration: 400 * (1+ i)}}>
       <span class='bg-primary h-3 w-3 rounded-full inline-block mr-2'></span>
      
       {item.name}
       </li>
       {/if}
       {/each}
   </ul>
   <Button>All Trip</Button>
</div>
<div class='h-full w-full  mt-10 sm:mt-0'>
    <img class='object-cover sm:h-auto h-64' src='/images/travel.png' alt="travel view">
</div>
</div>

</div>