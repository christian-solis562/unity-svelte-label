<svelte:options tag="unity-label" />

<script lang="ts">
    // pass in values from parent to update these props
    export let text = `default`;
    export let forvalue = `default`;

    // can't use dashed props at the moment
    // export let isDisabled = false;
    export let isdisabled = false;

    // this is a reactive statement
    $: labelText = `Text for this label is ${text}`
</script>

<label for={forvalue} disabled={isdisabled}>{text}</label>
