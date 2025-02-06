<script lang="ts">
    interface Props {
        children?: import('svelte').Snippet;
    }

    let { children }: Props = $props();
</script>

<thead>
    {@render children?.()}
</thead>

<style>
    thead {
        background-color: var(--gc-table-header-bg-color, var(--gc-secondary-color));
    }
</style>