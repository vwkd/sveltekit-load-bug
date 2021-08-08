<script>
    export let data;
    console.log("Mounted about component.");
</script>

<svelte:head>
    <title>About</title>
</svelte:head>

<h3>About</h3>

<p>Data: {data}</p>