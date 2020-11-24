<script>
    import Logo from './Logo.svelte'
    import Hero from '../Hero.svelte'
    import Sidebar from './sidebar.svelte'
    
 
</script>

<header class="bg-no-repeat banner-container md:h-screen">
    <nav class="flex  justify-between items-center sm:p-6 p-4 ">
            <Logo />
        <Sidebar />
       
    </nav>
    <div class="lg:px-32 sm:px-16 px-8 mx-auto h-full w-full">
        <Hero />
    </div>
   
</header>

<style>
  
    .banner-container {
    background-image:url("/images/bg1.png");
    background-size: cover;
    background-position: center ;
}
</style>