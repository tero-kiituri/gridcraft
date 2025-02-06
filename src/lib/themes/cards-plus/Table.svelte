<script lang="ts">
    interface Props {
        children?: import('svelte').Snippet;
    }

    let { children }: Props = $props();
</script>

<div class="max-w-full min-w-full">
    {@render children?.()}
</div>