<script>
    import ButtonContact from "../components/buttons/ButtonContact.svelte";
</script>

<div class="main_contacts w-full h-auto pb-4 pt-4">
    <div class="grid items-center justify-center apresentation-text-m">
        <div class="flex justify-around w-full">
            <ButtonContact title="WhatsApp" link="https://api.whatsapp.com/send?phone=996351318" color="green" icon="fa-brands fa-whatsapp" />
            <ButtonContact title="Linkedin" link="https://www.linkedin.com/in/matheus-marques-linhares-b5512b210" color="red" icon="fa-brands fa-linkedin-in" />
            <ButtonContact title="GitHub" link="https://github.com/mmarquesl583" color="black" icon="fa-brands fa-github" />
            <ButtonContact title="Email" link="mailto:matheus05linhares@hotmail.com" color="blue" icon="fa-solid fa-envelope" />
            <ButtonContact title="Instagram" link="https://instagram.com/markzada583" color="pink" icon="fa-brands fa-instagram" />
        </div>
    </div>
</div>