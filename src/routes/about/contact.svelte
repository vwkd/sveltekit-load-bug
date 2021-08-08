<script context="module">
    console.log("Prefetching about/contact component.");

    export async function load() {
        const data = `Hello from About/Contact!`;

        return {
            props: {
                data,
            },
        };
    }
</script>

<script>
    export let data;
    console.log("Mounted about/contact component.");
</script>

<svelte:head>
    <title>About/Contact</title>
</svelte:head>

<h3>About/Contact</h3>

<p>Data: {data}</p>
