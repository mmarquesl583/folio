<script>
    export let i_class = ""
    export let border_color
    export let color
    export let text

    let text_class
    let border_class = `rounded-lg border-${border_color} hover:scale-110`;
    let card_class = `text-${color} w-auto h-20 rounded-lg bg-gray-800 grid items-center justify-center hover:cursor-pointer transform transition-all duration-300  a`;
    if (i_class === "") {
      text_class = "text-2xl";
    } else {
      text_class = "text-xl";
      i_class += " centralize items-end"
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

<div class={border_class}>
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
</div>
