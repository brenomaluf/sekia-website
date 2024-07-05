<script>
    import { onMount } from "svelte";

    onMount(() => {
        window.addEventListener("scroll", handleScroll);

        return () => {
            window.removeEventListener("scroll", handleScroll);
        };
    });

    function handleScroll() {
        const video = document.getElementById("myVideo");
        
        if (video) {
            const offset = window.scrollY;
            video.style.transform = `translateY(${offset * 0.75}px)`;
        }
    }
</script>

<style>
    .video-container {
        height: 100vh;
        overflow: hidden;
        position: relative;
    }
    video {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
</style>

<div class="video-container">
    <video autoplay muted loop id="myVideo" class="w-full h-full object-cover">
        <source src="assets/rain.mp4" type="video/mp4" />
    </video>
    <div class="absolute inset-0 flex items-center justify-center text-center text-white">
        <div>
            <img src="assets/logo.png" alt="Logo" class="mb-4 w-44 mx-auto">
            <h2 class="text-4xl font-bold">Cresça sua empresa e aumente suas vendas com a Sekia</h2>
        </div>
    </div>
</div>
