<script>
    import TecCard from "../components/cards/TecCard.svelte";
</script>

<div class="main_tecnologies w-full h-auto p-16">
    <div class="grid items-center justify-center text-white apresentation-text-m">
        <span class="centralize">
            TECNOLOGIAS
        </span>
        <div class="mt-8 grid grid-cols-2 gap-3 sm:grid-cols-3 md:grid-cols-4 lg:grid-cols-5">
            <span class="col-span-2 sm:col-span-3 md:col-span-4 lg:col-span-5 text-2xl lg:text-3xl">Domino:</span>
            <TecCard border_color="gold" color="yellow" i_class="fa-brands fa-square-js" />
            <TecCard border_color="gold" color="green" i_class="fa-brands fa-node" />
            <TecCard border_color="gold" color="orange" text="Svelte" />
            <TecCard border_color="gold" color="green" i_class="fa-brands fa-vuejs" />
            <TecCard border_color="gold" color="purple" i_class="fa-brands fa-php" />
            <TecCard border_color="gold" color="blue" text="Docker" i_class="fa-brands fa-docker" />
            <TecCard border_color="gold" color="orange" text="WebSocket" />
            <TecCard border_color="gold" color="yellow" i_class="fa-solid fa-database" />
            <TecCard border_color="gold" color="white" i_class="fa-brands fa-linux" />
            <TecCard border_color="gold" color="white" i_class="fa-brands fa-git" />
            <TecCard border_color="gold" color="pink" i_class="fa-brands fa-sass" />
            <TecCard border_color="gold" color="blue" i_class="fa-brands fa-bootstrap" />
            <TecCard border_color="gold" color="red" text="Tailwind" />
            <TecCard border_color="gold" color="red" i_class="fa-brands fa-html5" />
            <TecCard border_color="gold" color="blue" i_class="fa-brands fa-css3-alt" />

            <span class="col-span-2 sm:col-span-3 md:col-span-4 lg:col-span-5 text-2xl lg:text-3xl text-gray-200">Conhecimentos Gerais:</span>
            <TecCard border_color="silver" color="red" text="CakePHP" />
            <TecCard border_color="silver" color="orange" i_class="fa-brands fa-python" />
            <TecCard border_color="silver" color="red" i_class="fa-brands fa-angular" />

            <span class="col-span-2 sm:col-span-3 md:col-span-4 lg:col-span-5 text-2xl lg:text-3xl text-gray-5000">Estudando:</span>
            <TecCard border_color="bronze" color="blue" i_class="fa-brands fa-react" />
            <TecCard border_color="bronze" color="green" text="Express" />
        </div>
    </div>
</div>