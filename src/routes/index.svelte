<script context="module">
    console.log("Prefetching index component.");

    export async function load() {
        const data = `Hello from Index!`;

        return {
            props: {
                data,
            },
        };
    }
</script>

<script>
    console.log("Mounted index component.");

    export let data;
</script>

<svelte:head>
    <title>Index</title>
</svelte:head>

<h3>Index</h3>

<p>Data: {data}</p>
