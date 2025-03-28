<script>
	import { onMount } from "svelte";

    let showText = false;

    onMount(() => {
        setTimeout(() => {
            showText = true;
        }, 100);
    });
</script>

<section class="introduction-container">
    <div class="centered">
        <div class="title-container">
            <h1>Hi, I'm Mohammed.</h1>
            {#if showText}
            <p class="typewriter">
                I'm a junior software engineer at 
                <a href="https://www.totalmerchandise.co.uk/" target="_blank" rel="noopener noreferrer">
                    Total Merchandise
                </a>.
            </p>
            {/if}
        </div>
    </div>
</section>

<style>
    .centered {
        display: flex;
        width: 100%;
        height: 100%;
        justify-content: center;
        align-items: center;
    }

    .introduction-container {
        display: flex;
        flex-direction: column;
        color: white;
        height: 60vh;
        width: 100%;
    }

    .title-container {
        display: flex;
        height: fit-content;
        padding: 15px;
        padding-top: 85px;
        flex-direction: column;
    }

    .title-container h1 {
        font-size: clamp(2.5em, 6.8vw, 8rem);
        margin: 0;
    }

    .typewriter {
        display: inline-block; /* Prevent full width */
        overflow: hidden;
        white-space: nowrap;
        border-right: 2px solid orange;
        width: 0;
        animation: typing 2.5s steps(50, end) forwards, blink-caret 0.75s step-end infinite;
    }

    @keyframes typing {
        from { width: 0 }
        to { width: 42ch; }
    }

    @keyframes blink-caret {
        from, to { border-color: transparent; }
        50% { border-color: orange; }
    }

    .title-container p {
        font-size: clamp(1.5rem, 2vw, 2rem);
    }

    .title-container a {
        font-weight: bold;
        color: #fcaa67;
    }
</style>