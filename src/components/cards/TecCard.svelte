<script>
    export let color = "blue";
    export let text;
    export let i_class = "";

    let text_class = "";
    let card_class = `text-${color} w-40 h-20 border-2 border-gray-400 rounded-lg bg-gray-800 grid items-center justify-center hover:cursor-pointer transform transition-all duration-300 hover:scale-110 a`;
    if (i_class === "") {
      text_class = "text-2xl";
    } else {
      text_class = "text-xl";
    }
    if (text) {
      i_class += " text-5xl";
    } else {
      i_class += " text-6xl";
    }


  </script>

  <style>
    .hover\:scale-110:hover {
      transform: scale(1.10);
    }
  </style>

  <div class={card_class}>
    {#if i_class != " text-5xl"}
    <i class={i_class}></i>
    {/if}
    {#if text}
    <span class={text_class}>
      {text}
    </span>
    {/if}
  </div>
