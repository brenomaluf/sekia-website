<script lang="ts">
	export let title: string = "default";
	export let subtitle: string = "default";
	export let srcImg: string = 'assets/livro.png';
</script>

<div class="contenta w-72 h-96 text-center items-center flex flex-col p-10 text-white rounded-3xl bg-card-gray">
	<h2 class="font-bold text-3xl m-1" >{title}</h2>
	<h3 class="font-normal text-sm m-1">{subtitle}</h3>
	<img class="size-48" src={srcImg} alt="" />
</div>
