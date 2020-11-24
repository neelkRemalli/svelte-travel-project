<script>
    import HeaderSection from './HeaderSection.svelte'
</script>


<div class='mt-40'>
    <HeaderSection title='Contact' />
    <div class='h-bg relative'>
       
    <div style="background-image: url('/images/bgContact.jpg');" class='smallHeight bg-cover bg-center bg-fixed' >
    
        <div class='contactInbox bg-white absolute bottom-0 right-0 sm:mr-40 mr-10 mb-2 shadow-2xl rounded p-6 text-center'>
           <h1 class='uppercase text-gray-900 font-bold my-6'> the best of the tour info delevered to your box </h1>
           <p class='text-sm pt-8'>subscribe to more inspiring places in the world</p>
           <input class='block mt-8 outline-none border border-gray-500 p-2 w-full rounded' type="email" placeholder="Your Email">
           <button class='transition duration-500 ease-in-out inline-block mt-6 text-primary text-xl font-bold hover:text-orange-800 hover:underline'>Subscribe </button>
        </div>
        
    </div>
    </div>
    </div>


    <style>
        .smallHeight{
            height: 90%;
        }
        .contactInbox{
            height: 400px;
            width: 320px;
        }
        @media only screen and (max-width: 640px) {
            .contactInbox{
            height: 380px;
            width: 250px;
        }
        
      }
    </style>











