<script>
    import Spongebob from "$lib/assets/Spongebob.jpeg"
</script>

<div class="main-page">
    <h1>Welcome to DeeperRoute</h1>
    <img src={Spongebob} alt="Alt Spongebob">
    <a href="/">Go to main page</a>
    <a href="/testRoute/BeneathTestRoute">Go Deeper!</a>    
</div>

<style>
    .main-page {
        display: flex;
        flex-direction: column;
        align-items: center;
        height: 100%;
        gap: 2rem;
    }
    img {
        max-width: 15rem;
        aspect-ratio: 1/1;
        object-fit: cover;
        object-position: top;
        border-radius: 100%;
        border: 10px solid rgb(120, 211, 184);
    }
</style>