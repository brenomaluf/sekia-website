<script lang="ts">
	export let img: string = 'assets/chatIcon.png';
	export let text: string = 'Entramos em contato para nosso diagnóstico de marca gratuito';
</script>

<div>
	<div
		class="rounded-3xl w-[200px] h-[200px] bg-card-gray flex justify-center sm:my-0 my-5 items-center mx-auto"
	>
		<img src={img} alt="" width="150" height="150" />
	</div>
	<p class="font-bold sm:w-[250px] w-full px-5 text-center pt-3 text-lg">{text}</p>
</div>
