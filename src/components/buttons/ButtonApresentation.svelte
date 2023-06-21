<script>
  import { tweened } from 'svelte/motion';
  import { cubicOut } from 'svelte/easing';

  let hoverAnimation = tweened(10, {
    duration: 300,
    easing: cubicOut,
  });
  function handleMouseOver() {
    hoverAnimation.set(20);
  }
  function handleMouseOut() {
    hoverAnimation.set(10);
  }

  export let type = "linkedin"
  let i_class = "h-5 w-5 text-orange-200 text-6xl "
  switch(type){
    case "github":
    i_class += "fa-brands fa-github"
        break
    case "doc":
    i_class += "fa-solid fa-file-lines"
        break
    default:
    i_class += "fa-brands fa-linkedin"
  }
</script>

<style>
  .box {
    transition: transform 0.3s;
  }
  .box:hover{
    cursor: pointer;
  }
</style>

<!-- svelte-ignore a11y-mouse-events-have-key-events -->
<div
  class="box centralize"
  on:mouseover={handleMouseOver}
  on:mouseout={handleMouseOut}
  style="transform: translateY({-$hoverAnimation}px);"
>
  <i class={i_class}></i>
</div>
