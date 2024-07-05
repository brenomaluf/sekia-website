<script lang="ts">
	export let img: string = 'assets/chatIcon.png';
	export let text: string = 'Entramos em contato para nosso diagnóstico de marca gratuito';
</script>

<div>
	<div class="rounded-3xl w-[200px] h-[200px] bg-card-gray flex justify-center items-center mx-auto">
		<img src={img} alt="" width="150" height="150" />
	</div>
	<p class="font-bold w-[250px] text-center pt-3 text-lg">{text}</p>
</div>
