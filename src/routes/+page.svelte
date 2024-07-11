<script>
	import NavBar from '../components/NavBar.svelte';
	import VideoSection from '../components/VideoSection.svelte';
	import Carroussel from '../components/Carroussel.svelte';
	import Footer from '../components/Footer.svelte';
	import Banner from '../components/Banner.svelte';
	import BigText from '../components/BigText.svelte';
	import TipsCard from '../components/TipsCard.svelte';
</script>

<main class="bg-black text-white min-h-screen m-0 p-0 font-sans">
	<NavBar></NavBar>
	<VideoSection></VideoSection>
	<BigText></BigText>
	<Carroussel></Carroussel>
	<Banner></Banner>
	<div class="sm:flex-row w-full flex-col flex justify-center sm:px-32 pb-8">
		<div class="sm:flex-row flex-col flex justify-center">
			<TipsCard img="assets/chatIcon.png" text="Envie seu contato"></TipsCard>
			<TipsCard
				img="assets/profileIcon.png"
				text="Entramos em contato para nossa avaliação gratuita"
			></TipsCard>
			<TipsCard img="assets/boxIcon.png" text="Entrega de soluções prontas para crescer sua empresa"
			></TipsCard>
		</div>
	</div>
	<Footer></Footer>
</main>

<style>
	@import url('https://fonts.googleapis.com/css2?family=SF+Pro+Display:wght@400;500;600;700&display=swap');

	.font-sans {
		font-family: 'SF Pro Display', sans-serif;
	}
	:global(body) {
		background-color: black;
	}
</style>
