<script>
	let { children } = $props();
</script>

<nav style="position:fixed; display:flex; flex-direction:column;">
	<a class="link-headers" href="/" style="margin-bottom: 100px">HOME</a>
	<a class="link-headers" href="/aboutme">ABOUT</a>
</nav>

{@render children()}

<style>
    @import '$lib/styles.css';

    .link-headers {
        margin: auto;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 36px;
        margin-top: -40px;
        width: fit-content;
        text-align: center;
        width: 70%
    }
</style>