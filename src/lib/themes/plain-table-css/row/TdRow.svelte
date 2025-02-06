<script lang="ts">
    interface Props {
        children?: import('svelte').Snippet;
    }

    let { children }: Props = $props();
</script>

<td class="gc-td">
    {@render children?.()}
</td>

<style>
    .gc-td {
        padding: var(--gc-td-padding, 0.5rem 0.75rem);
        text-align: var(--gc-td-text-align, left);
    }
</style>