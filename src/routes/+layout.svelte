<style>
    .layout-container {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        line-height: 50px;
        height: 50px;
        margin-top: 150px;
        background: red;
        border: red;
        border-top-width: 10px;
        border-style: solid;
        border-bottom-width: 10px;
    }

    .logo-link {
        display: flex;
        justify-self: center;
        align-content: center;
        height: 100%;
        margin-left: 5%
    }

    .logo-img {
        height: 151.8px;
        width: 216px;
        margin-top: -50px;
    }

    .nav-links-container {
        display: flex;
        justify-content: space-around;
        margin-left: 5%;
        width: 100%
    }

    .nav-link {
        padding-left: max(10px, 2%);
        padding-right: max(10px, 2%);
        color: white;
        font-weight: bold;
        letter-spacing: 1px;
        border-right: 3px solid white;
        width: 100%
    }

    .nav-img-container {
        width: 50px;
    }

    .nav-img {
        height: 100%;
    }
</style>

<nav class="layout-container">
    <!-- <div class="logo-container"> -->
        <a class="logo-link" href="/" id="currpage">
            <img class="logo-img" src="/logo.png">
        </a>
    <!-- </div> -->
    <div class="nav-links-container">
        <a class="nav-link" href="/staff">STAFF</a>
        <a class="nav-link" href="/archive">ARCHIVE</a>
        <a class="nav-link" href="/releases">RELEASES</a>
        <a class="nav-link" href="https://store.anisonhijack.moe">STORE</a>
        <a class="nav-link" href="/donate">DONATE</a>
        <a class="nav-link" href="/contact">CONTACT</a>
        <span class="nav-img-container" style="flex: 0.5; display: flex">
            <a href="https://linktr.ee/anisonhijack" target="_blank">
                <img class="nav-img" src="/social/generic.png" alt="Linktree">
            </a>
        </span>
    </div>
</nav>

<slot></slot>