<nav>
    <div class="nav-container">
        <div class="nav-links">
            <a href="/">Home</a>
            <a href="#about">About</a>
            <a href="#timeline">Timeline</a>
        </div>
    </div>
</nav>

<style>
    nav {
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        width: 100%;
        height: 50px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: black;
        color: white;
        z-index: 1000;
        padding: 10px 0;
    }

    .nav-links a {
        color: black;
        text-decoration: none;
        font-size: 0.9rem;
        margin: 0 15px;
        background-color: #fcaa67;
        padding: 10px;
        border-radius: 20px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    }

    .nav-links a:hover {
        color: white;
    }
</style>
