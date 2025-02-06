<script lang="ts">
    interface Props {
        children?: import('svelte').Snippet;
    }

    let { children }: Props = $props();
</script>

<div class="grid grid-cols-2 md:grid-cols-3 gap-4 mt-4">
    {@render children?.()}
</div>