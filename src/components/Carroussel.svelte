<script>
	import SolutionCard from './SolutionCard.svelte';
	let cards = [
		{
			title: 'anúncios online',
			desc: 'Criação de anúncios em redes sociais, direcionado para seus clientes ideiais',
			src: 'assets/tag.png'
		},
		{
			title: 'design e marca',
			desc: 'Trabalho de branding completo que encanta e fideliza seus clientes do começo ao fim',
			src: 'assets/pincel.png'
		},
		{
			title: 'criação de conteúdo',
			desc: 'Criação de conteúdo que gera valor a sua marca, retendo seus clientes, e atraindo novos',
			src: 'assets/livro.png'
		}
	];
</script>

<div class="flex justify-center mx-auto gap-12 pt-12 pb-12">
	{#each cards as { title, desc, src }}
		<SolutionCard {title} subtitle={desc} srcImg={src}></SolutionCard>
	{/each}
</div>

