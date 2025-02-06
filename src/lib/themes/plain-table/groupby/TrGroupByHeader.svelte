<script lang="ts">
    interface Props {
        children?: import('svelte').Snippet;
    }

    let { children }: Props = $props();
    // export let isSelected = false;
</script>

<tr>
    {@render children?.()}
</tr>