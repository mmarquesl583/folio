<script>
    import ButtonContact from "../components/buttons/ButtonContact.svelte";
</script>

<div class="main_contacts w-full h-auto pb-4 pt-4">
    <div class="grid items-center justify-center apresentation-text-m">
        <div class="flex justify-around w-full">
            <ButtonContact title="WhatsApp" color="green" icon="fa-brands fa-whatsapp" />
            <ButtonContact title="Linkedin" color="red" icon="fa-brands fa-linkedin-in" />
            <ButtonContact title="GitHub" color="black" icon="fa-brands fa-github" />
            <ButtonContact title="Email" color="blue" icon="fa-solid fa-envelope" />
            <ButtonContact title="Instagram" color="pink" icon="fa-brands fa-instagram" />
            <!-- <a href="https://api.whatsapp.com/send?phone=27996351318&text=Olá%2C%20gostaria%20de%20saber%20mais%20informações." target="_blank">
                .
            </a> -->
        </div>
    </div>
</div>