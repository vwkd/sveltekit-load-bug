<script>
    export let data;
    console.log("Mounted layout component.");
</script>

<header>
    <nav>
        <a href="/">Index</a>
        <a href="/about">About</a>
        <a href="/about/contact">About/Contact</a>
        <a href="/incorrect">Incorrect</a>
    </nav>
</header>

<p>Data: {data}</p>

<main>
    <slot />
</main>

<style>
    :global(html) {
        background-color: rgb(233, 246, 238);
    }

    main {
        background-color: rgb(225, 230, 255);
    }
</style>
