<script>
    import Logo from "$lib/ui/svgs/branding/brand-logo.svelte";
    import AccountMenu from "$lib/ui/avatar/AccountMenu.svelte";
</script>

<div>
    <nav>
        <Logo />
        <a href="/">Home</a>
        <a href="/">Ipsum</a>
        <a href="/">Dolor</a>
        <a href="/">Amet</a>
    </nav>
    <AccountMenu /><!--Pfp&Icons for user settings-->
</div>

<style>
    div {
        height: 100vh;
        flex: 1;
        display: flex;
        flex-direction: column;
        align-items: end;
        box-sizing: border-box;
        padding: 16px 22px 16px 32px;
    }
    
    nav {
        height: 100%;
        display: flex;
        flex-direction: column;
    }

    a {
        font-family: "Work Sans", sans-serif;
        font-size: 1.4rem; /*Need to change that*/
        font-weight: 700;
        text-transform: uppercase;
    }
</style>