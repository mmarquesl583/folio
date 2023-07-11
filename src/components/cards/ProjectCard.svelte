<script>
    import MockupNanapro from "../../../public/card_img/mockup-nanapro.png"
    import Mockup from "../../../public/card_img/mockup.png"

    export let nanapro
    export let link

    function openNewWindow(url) {
        window.open(url, "_blank");
    }
</script>

<div on:click={openNewWindow(link)}>
    {#if nanapro}
    <img src={MockupNanapro}>
    {:else}
    <img src={Mockup}>
    {/if}
</div>

<style>
    @property --a { /* control the gradient rotation (no need to update) */
    syntax: "<angle>";
    initial-value: 45deg;
    inherits: true;
    }
    @property --r {
    syntax: "<angle>";
    initial-value: 5deg; /* control the image rotation */
    inherits: true;
    }
    @property --p { /* control the color stops of the gradient (no need to update) */
    syntax: "<percentage>";
    initial-value: 0%;
    inherits: true;
    }
    img {
    --c: #ffffff; /* the main coloration of the rotating gradient */
    width: 500px; /* the size of the image*/
    height: 350px;
    aspect-ratio: 1;
    border-radius: 25px;
    border: 4px solid #0000; /* the thickness for the rotating gradient */
    padding: 10px; /* the gap */
    background:
        conic-gradient(from var(--a),
        #0000 calc(100% - var(--p)),
        var(--c) calc(100% - var(--p)) calc(100% + var(--p)),
        #0000 calc(100% + var(--p))) border-box;
    --g: linear-gradient(#000 0 0);
    -webkit-mask:
        var(--g),var(--g) padding-box,
        conic-gradient(from var(--a),
        #000d calc(30% - var(--p)),
        #000  calc(50% - var(--p)) calc(50% + var(--p)),
        #000d calc(70% + var(--p))) content-box;
    -webkit-mask-composite: xor;
    transition: --p .5s,--r .4s;
    cursor: pointer;
    --p: 100%
    }
</style>