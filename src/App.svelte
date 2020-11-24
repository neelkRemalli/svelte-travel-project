<script>
import Navbar from './components/navbar/Navbar.svelte'

import Trip from './components/Trip.svelte'
import BackgroundDiscover from './components/BackgroundDiscover.svelte'
import TravelTips from './components/TravelTips.svelte'
import Contact from './components/Contact.svelte'
import Footer from './components/Footer.svelte'



</script>
<div id='home'>
	<Navbar />
</div>
<div id='service' class='lg:max-w-screen-lg mx-auto '>
	<Trip />	
</div>
<BackgroundDiscover />
<div id='travel' class='lg:max-w-screen-lg mx-auto '>
	<TravelTips />	
</div>
<div id='contact'>
	<Contact />
</div>
<Footer />



<style>
	
	:global(body){
		padding: 0;
		margin: 0;
		box-sizing: border-box;
		font-family: 'Alegreya', serif;
	
		
	}
</style>