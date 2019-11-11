<script>
	export let name;
	import Counter from './Counter.svelte'
	import AddNumber from './AddNumber.svelte'
	import Info from './Info.svelte'
	import LoginStatus from './LoginStatus.svelte'

		const pkg = {
			name: 'svelte',
			version: 3,
			speed: 'blazing',
			website: 'https://svelte.dev'
		};
</script>

<h1 class="welcome-name">Welcome {name}!</h1>
<Counter />
<AddNumber />
<Info {...pkg}/>
<LoginStatus />
