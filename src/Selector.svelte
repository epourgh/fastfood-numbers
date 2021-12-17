<script>
    import { getContext, setContext } from 'svelte'

    const selected = getContext('selected')

	function handleClick(value) {
        $selected = value;
	}
    
</script>

<button value='chipotle' on:click={() => handleClick('chipotle') }>
	Chipotle
</button>

<button value='subway' on:click={() => handleClick('subway') }>
	Subway
</button>

<p>{$selected}</p>