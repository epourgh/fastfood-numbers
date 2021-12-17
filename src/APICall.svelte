<script>
    import { getContext } from 'svelte'
    const selected = getContext('selected')
</script>

{#if $selected !== 'empty'}
https://placeholder.name/{$selected}
{/if}