<svelte:options tag="unity-label" />

<script lang="ts">
    // cant use dashed props at the moment
    export let text = `default`;
    export let forvalue = `default`;
    export let isDisabled = false;
</script>

<label for={forvalue} disabled={isDisabled}>{text}</label>
