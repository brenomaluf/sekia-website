<script lang="ts">
	import MenuButton from "./MenuButton.svelte";

	export let cta: string = "default";
	export let srcImg: string = 'default';
</script>

<div class="relative w-full">
    <div class="absolute inset-0 flex flex-col items-center justify-center">
        <h2 class="text-white text-5xl font-bold mb-4">{cta}</h2>
        <div class="list-none mt-5 text-lg">
            <MenuButton></MenuButton>
        </div>
        
    </div>
    <img src="{srcImg}" alt="" class="w-full">
</div>
