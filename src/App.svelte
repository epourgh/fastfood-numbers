<script>
	import { setContext } from 'svelte'
    import {writable} from 'svelte/store';

	import Selector from './Selector.svelte';
	import APICall from './APICall.svelte';

	let selected = writable('empty');
	setContext('selected', selected)

	let name = 'Emerson';
</script>

<h1 class="text-3xl font-bold underline">Welcome back, {name}</h1>

<Selector />
<APICall />