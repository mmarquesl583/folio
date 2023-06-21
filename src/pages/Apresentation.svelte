<script>
    import ButtonApresentation from "../components/buttons/ButtonApresentation.svelte";
</script>

<div class=" centralize w-full h-full">
    <div class="grid items-center justify-center apresentation-text-m  w-full">
        <span class="apresentation-text-t ">OI, EU SOU O MATHEUS</span>
        <div class="apresentation-text-m flex">
            REACT
            <div class="flex items-center justify-around w-full">
                <ButtonApresentation />
                <ButtonApresentation type="github" />
                <ButtonApresentation type="doc" />
            </div>
        </div>
        <span class="apresentation-text-m ">DEVELOPER</span>
        <span class="apresentation-text-b ">
            TENHO DOIS ANOS DE EXPERIÊNCIA COMO DESENVOLVEDOR FRONT-END
        </span>
        <span class="apresentation-text-b ">
            TRABALHO COMO CLT E FREELANCER.
        </span>
    </div>
</div>