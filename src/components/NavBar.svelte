<script>
	import MenuButton from './MenuButton.svelte';
	import MenuItem from './MenuItem.svelte';
	// @ts-ignore
	import MenuLogo from './MenuLogo.svelte';

	let item = [
		{
			name: 'Tecnologia',
			href: 'https://google.com'
		}
	];
</script>

<nav class="bg-transparent fixed z-10 w-full">
	<div class="w-full px-4 py-3 mx-auto">
		<div class="flex justify-between items-center">
			<ul class="flex items-center space-x-8">
				<MenuLogo></MenuLogo>
			</ul>
			<ul class="flex items-center space-x-4 text-lg">
				<!-- {#each item as { name, href }}
					<MenuItem {name} {href}></MenuItem>
				{/each} -->
				<MenuButton></MenuButton>
			</ul>
		</div>
	</div>
</nav>
