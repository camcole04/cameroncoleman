<script>
	let { children } = $props();
</script>

<nav class="menu-nav">
	<h2 class="menu-header">QUICK LINKS</h2>
	<a class="menu-link" href="/" style="margin-bottom: 40px;">HOME</a>
	<a class="menu-link" href="/aboutme" style="margin-bottom: 40px;">ABOUT ME</a>
	<a class="menu-link" href="/projects" style="margin-bottom: 40px;">PROJECTS</a>
</nav>

{@render children()}

<style>
    @import '$lib/styles.css';

    .menu-nav {
        position: fixed;
        display: flex;
        flex-direction: column;
        background-color: #f5f1e9; /* light cream */
        padding: 40px 30px;
        height: 100vh;
        width: 220px;
        box-shadow: 4px 0 10px rgba(0,0,0,0.1);
        border-right: 2px solid #d2b48c; /* tan for border */
        font-family: 'Georgia', serif;
    }

    .menu-header {
        font-family: 'Palatino Linotype', 'Book Antiqua', Palatino, serif;
        font-size: 48px;
        color: #8b4513; /* brown */
        margin-bottom: 60px;
        text-align: center;
        letter-spacing: 3px;
        border-bottom: 2px solid #d2b48c;
        padding-bottom: 10px;
    }

    .menu-link {
        font-family: 'Georgia', serif;
        font-size: 28px;
        color: #5a3e1b; /* dark brown */
        text-decoration: none;
        margin-bottom: 30px;
        text-align: center;
        transition: color 0.3s ease;
    }

    .menu-link:hover {
        color: #a0522d; /* sienna */
        text-decoration: underline;
    }
</style>
