<script>
    const PhoneLogo = '/images/phoneLogo.svg'
    const SocialMediaLogo = [
        {image: '/images/facebook.svg'},
        {image: '/images/twitter.svg'},
        {image: '/images/linkin.svg'},
        {image: '/images/instgram.svg'},
    ]

</script>


<div class='bg-terniary p-12 mt-20 '>
    <div class="lg:max-w-screen-lg mx-auto flex sm:flex-row flex-col sm:justify-between sm:items-center text-gray-200 pb-2 border-b border-gray-800" > 
        <div class="flex items-center" >
            <img src={PhoneLogo} alt="phone">
            <span class='inline-block ml-2 text-gray-400'>(201) 555-0124</span>
        </div>
        <div class='flex sm:flex-row flex-col sm:items-center'>
            <h2 class='uppercase text-gray-400 text-sm my-4 sm:my-0'>fellow us on social media</h2>
            <ul class='flex sm:ml-2 sm:mb-0 mb-2'>
                {#each SocialMediaLogo as logo}
                <li class=' mr-4 sm:ml-2'>
                    <img src={logo.image} alt={logo.image}>
                </li>
                {/each}
            </ul>
        </div>
    </div>
    <div class='lg:max-w-screen-lg mx-auto text-gray-600 text-sm flex sm:flex-row flex-col sm:justify-between sm:items-center py-2'>
        <p class='my-2 sm:my-0'>2118 Thornridge Syracuse,Connecticut 35624</p>
        <p>created by neelkRemalli all right and privacy policy  reserved</p>
    </div>
</div>