<script>
    import TecCard from "../components/cards/TecCard.svelte";
</script>

<div class="main_tecnologies w-full h-auto p-16">
    <div class="grid items-center justify-center text-white apresentation-text-m">
        <span class="centralize">
            TECNOLOGIAS
        </span>
        <div class="mt-8 grid grid-cols-2 gap-3 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5">
            <TecCard color="yellow" i_class="fa-brands fa-square-js" />
            <TecCard color="green" i_class="fa-brands fa-node" />
            <TecCard color="orange" text="Svelte" />
            <TecCard color="blue" i_class="fa-brands fa-react" />
            <TecCard color="green" i_class="fa-brands fa-vuejs" />
            <TecCard color="red" i_class="fa-brands fa-angular" />
            <TecCard color="green" text="Express" />
            <TecCard color="purple" i_class="fa-brands fa-php" />
            <TecCard color="red" text="CakePHP" />
            <TecCard color="orange" i_class="fa-brands fa-python" />
            <TecCard text="Docker" i_class="fa-brands fa-docker" />
            <TecCard color="orange" text="WebSocket" />
            <TecCard color="yellow" i_class="fa-solid fa-database" />
            <TecCard color="white" i_class="fa-brands fa-linux" />
            <TecCard color="white" i_class="fa-brands fa-git" />
            <TecCard color="pink" i_class="fa-brands fa-sass" />
            <TecCard color="blue" i_class="fa-brands fa-bootstrap" />
            <TecCard color="red" text="Tailwind" />
            <TecCard color="red" i_class="fa-brands fa-html5" />
            <TecCard color="blue" i_class="fa-brands fa-css3-alt" />
          </div>

    </div>
</div>