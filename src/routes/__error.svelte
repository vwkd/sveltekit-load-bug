<script context="module">
    console.log("Prefetching error component.");

    export async function load() {
        const data = `Hello from Error!`;

        return {
            props: {
                data,
            },
        };
    }
</script>

<script>
    export let data;
    console.log("Mounted error component.");
</script>

<svelte:head>
    <title>Error</title>
</svelte:head>

<h3>Error</h3>

<p>Data: {data}</p>
