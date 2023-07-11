<script>
    import ButtonContact from "../components/buttons/ButtonContact.svelte";
</script>

<div class="main_contacts w-full h-auto p-16">
    <div class="grid items-center justify-center apresentation-text-m">
        <span class="centralize text-8xl">
            CONTATOS
        </span>
        <div class="flex justify-around">
            <ButtonContact title="WhatsApp" color="green" icon="fa-brands fa-whatsapp" />
            <ButtonContact title="Linkedin" color="red" icon="fa-brands fa-linkedin-in" />
            <ButtonContact title="GitHub" color="black" icon="fa-brands fa-github" />
            <ButtonContact title="Email" color="blue" icon="fa-solid fa-envelope" />
            <ButtonContact title="Instagram" color="pink" icon="fa-brands fa-instagram" />
        </div>
    </div>
</div>