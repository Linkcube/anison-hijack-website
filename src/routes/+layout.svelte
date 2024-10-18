<style>
    .layout-container {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        line-height: 40px;
        height: 40px;
        margin-top: 150px;
        background: red;
        border: red;
        border-top-width: 10px;
        border-style: solid;
        border-bottom-width: 10px;
        min-width: 530px;
        margin-bottom: 120px;
    }

    .logo-link {
        display: flex;
        justify-self: center;
        align-content: center;
        height: 100%;
        margin-left: 5%
    }

    .logo-img {
        height: calc(1518px * .2);
        width: calc(2160px * .2);
        margin-top: -125px;
    }

    .nav-links-container {
        display: flex;
        justify-content: space-around;
        width: 100%
    }

    .nav-link {
        color: white;
        font-weight: bold;
        letter-spacing: 1px;
        border-right: 3px solid white;
        width: 100%;
        text-decoration: none;
        display: flex;
        justify-content: center;
        margin-top: auto;
        margin-bottom: auto;
    }

    .nav-link:hover {
        text-decoration-line: underline;
        text-decoration-thickness: auto;
    }

    .nav-img {
        height: 100%;
        width: 40px;
    }

    @media (max-width: 1100px) {
        .logo-img {
            height: calc(1518px * .1);
            width: calc(2160px * .1);
            margin-top: -50px;
        }

        .logo-link, .nav-links-container {
            margin-left: 0;
        }

        .layout-container {
            margin-bottom: 50px;
        }
    }

    @media (max-width: 800px) {
        .logo-img {
            display: none;
        }

        .layout-container {
            margin-bottom: 0px;
        }
    }
</style>

<nav class="layout-container">
    <a class="logo-link" href="/" id="currpage">
        <img class="logo-img" src="/logo.png">
    </a>
    <div class="nav-links-container">
        <a class="nav-link" href="/staff">STAFF</a>
        <a class="nav-link" href="/archive">ARCHIVE</a>
        <a class="nav-link" href="/releases">RELEASES</a>
        <a class="nav-link" href="https://store.anisonhijack.moe">STORE</a>
        <a class="nav-link" href="/donate">DONATE</a>
        <a class="nav-link" href="/contact">CONTACT</a>
        <a href="https://linktr.ee/anisonhijack" target="_blank">
            <img class="nav-img" src="/social/generic.png" alt="Linktree">
        </a>
    </div>
</nav>

<slot></slot>