<script>
    import Button from './Button.svelte'
    import HeaderSection from './HeaderSection.svelte'
    import {fade, fly} from 'svelte/transition'
    const TripImageLeft = 'images/trip1.jpg' 
    const RightImageUpper = 'images/rightUpper.jpg' 
    const RightImageBotton = 'images/rightButton.jpg' 
   let y;

</script>
<svelte:window bind:scrollY={y} />
<div class='my-20'>
    <HeaderSection title='Dream Your Next Trip' />
   

<div class=' grid md:grid-cols-3  grid-cols-1 md:px-4 px-8 gap-1 w-full '>
    {#if y >= 300}
    <div class='bg-secondary col-span-2 flex sm:flex-row flex-col overflow-hidden rounded-t-lg ' transition:fly="{{x: -200, delay: 300, duration: 2000 }}" >
        <img class='sm:w-1/3 sm:h-auto h-56  ' src={TripImageLeft} alt="side view">
      <div class='self-center p-12'>
          <p class='text-gray-800 font-bold text-lg'>You Can Swim With Whales Under the Midnight
           Sun Thanks to This Epic New Tour in Iceland.</p>
           <Button>Learn More</Button>
      </div>
    </div>
  {/if}
<!------>
{#if y >= 300}
    <div class=' md:grid md:grid-cols-1  gap-1 h-full'  transition:fly="{{x: 200, delay: 500, duration: 2000 }}">
     <div class='flex items-center bg-secondary '>
            <img class='w-1/2 h-full object-cover' src={RightImageUpper} alt="upper right tour">
        <p class='md:px-2 p-4 lg:text-base text-sm font-bold text-gray-800 '>National Park Forests, Amazing Wildlife,
              and It’s Best Explored by Water</p>
     </div>
     <div class=' flex items-center bg-secondary mt-1 md:mt-0'>
           <img class='w-1/2 h-full object-cover' src={RightImageBotton} alt="upper right tour">
        <p class='md:px-2 p-4 lg:text-base text-sm font-bold text-gray-800 '>This Stunning Montana Tree  
            and Real-life Snow Globe in the Winter </p>
     </div>
    </div>
    {/if}
</div>
</div>

































<!-- <div class='mb-20 h-64 '>
   
    <div class='grid grid-cols-3 bg-blue-200 gap-4 '> 

        <div class='col-span-2 flex bg-blue-200 items-center'>
           <div class='w-1/3 h-auto'>
               <img class='' src={TripImageLeft} alt='sea tour'>
           </div>
           <div class='w-2/3 h-auto p-12  '>
               <p class='mb-4'>You Can Swim With Whales Under the Midnight
                    Sun Thanks to This Epic New Tour in Iceland
                </p>
               <Button >Learn More</Button>
           </div>
        </div>

        <div class='col-span-1 bg-blue-400'>
           <div class='flex'>
               <div class='w-1/2'>
                   <img class=' inline-block' src={RightImageUpper} alt="upper right tour">
               </div>
               <p>National Park Forests, Amazing Wildlife, and
                    Incredible Shipwrecks and It’s Best Explored by Water</p>
           </div>
           <div class='flex'>
               <div class='w-1/2'>
                   <img src={RightImageBotton} alt="upper right tour">
               </div>
               <p>This Stunning Montana Tree House Looks 
                   Like a Real-life Snow Globe in the Winter </p>
           </div>
        </div>
    </div>
</div> -->