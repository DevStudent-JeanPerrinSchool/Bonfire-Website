<script>
    import src from '$lib/ui/default_avatar.png';
    import MoreVertical from '../svgs/icons/more-vertical.svelte';
</script>

<div class="main">
    <a href="/" class="friendImg"> <img {src} alt="It's <username> ! <username> is beautiful • ᵕ •"> </a>
    <div class="txt">
        <p>Username</p>
        <span>@Username</span>
    </div>
    <a href="/" class="icon"> <MoreVertical /> </a>
</div>

<style>
    .main {
        display: flex;
        gap: 12px;
        align-items: center;
        padding: 8px;
        border-radius: 999px;
        transition: .15s !important;
    }

    .txt { display:block; }

    img, .userImg {
        width: 48px;
        height: 48px;
        border-radius: 99px;
    }

    p, span {
        font-family: "Work Sans", sans-serif;
        font-size: 1.1rem;
        letter-spacing: -0.02em;
    }

    .icon {
        display: flex;
        width: 52px;
        align-items: center;
        justify-content: center;
        cursor: default;
    }

    @media (prefers-color-scheme: dark) {
        .main:hover { background-color: #FFFFFF0D !important; }   
        span { color: #f1f8fe80; }
    }
    @media (prefers-color-scheme: light) {
        .main:hover { background-color: #1100000D !important; } 
        span { color: #00000080; }
    }
</style>