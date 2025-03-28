<script>
    import Navbar from "../components/navbar/+navbar.svelte";
    import Introduction from "../components/page_sections/+introduction.svelte";
    import About from "../components/page_sections/+about.svelte";
    import Timeline from "../components/page_sections/+timeline.svelte";
    import Footer from "../components/footer/+footer.svelte";

    export let introBackgroundColour = 'black';
    export let aboutBackgroundColour = '#fcaa67';
    export let timelineBackgroundColour = 'black';
    export let footerBackgroundColour = '#fcaa67';
</script>

<div class="page">

    <Navbar />
    <div class="page-section" style="background-color: {introBackgroundColour}">
        <Introduction />
    </div>
    <div class="page-section" style="background-color: {aboutBackgroundColour}">
        <About />
    </div>
    <div class="page-section" style="background-color: {timelineBackgroundColour}">
        <Timeline />
    </div>
    <Footer />

</div>


<style>

    .page {
        display: grid;
        flex-direction: column;
        margin: 0;
        padding: 0;
        font-family: 'Arial', sans-serif;
    }


</style>