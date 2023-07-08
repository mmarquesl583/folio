<script>
    import ButtonApresentation from "../components/buttons/ButtonApresentation.svelte";
    import ScrollAnimation from "../components/shared/ScrollAnimation.svelte";
    let scroll_display
    setTimeout(() => {
        scroll_display = true
    }, 2000);
</script>

<div class="main_apresentation centralize w-full h-full">
    <div class="pl-4 grid items-center justify-center apresentation-text-m  w-full">
        <span class="apresentation-text-t ">
            OI, EU SOU O MATHEUS
        </span>
        <div class="flex">
            <span class="text-yellow-500">
                J
            </span>
            <span class="text-yellow-500">
                S
            </span>
            CRIPT
            <div class="hidden items-center justify-around w-full md:flex">
                <ButtonApresentation />
                <ButtonApresentation type="github" />
                <ButtonApresentation type="doc" />
            </div>
        </div>
        <span class="apresentation-text-m ">DEVELOPER</span>
        <span class="apresentation-text-b ">
            TENHO DOIS ANOS DE EXPERIÊNCIA COMO DESENVOLVEDOR FULL-STACK
        </span>
        <span class="apresentation-text-b ">
            TRABALHO COMO CLT E FREELANCER.
        </span>
    </div>
    {#if scroll_display}
        <div class="absolute bottom-28">
            <ScrollAnimation />
        </div>
    {/if}
</div>
