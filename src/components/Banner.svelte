<script>
    import BannerImg from "./BannerImg.svelte";
    let banners = [
        {
            cta: 'Vamos discutir seu projeto?',
            srcImg: 'assets/banner1.png',
        },
    ]
</script>

<div>{#each banners as {cta, srcImg} }
    <BannerImg cta={cta} srcImg={srcImg}></BannerImg>
{/each}
</div>