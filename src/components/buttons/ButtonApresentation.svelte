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

  let link = "#"
  let i_class = "h-5 w-5 text-orange-200 text-4xl lg:text-5xl hover:text-orange-100 "

  switch(type){
    case "github":
      i_class += "fa-brands fa-github"
      link = "https://github.com/mmarquesl583"
    break
    case "doc":
      i_class += "fa-solid fa-file-lines"
      link = ""
    break
    default:
      i_class += "fa-brands fa-linkedin"
      link = "https://www.linkedin.com/in/matheus-marques-linhares-b5512b210"
  }
  function openNewWindow(url) {
    window.open(url, "_blank");
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
<!-- svelte-ignore a11y-click-events-have-key-events -->
<div
  class="box centralize"
  on:mouseover={handleMouseOver}
  on:mouseout={handleMouseOut}
  on:click={openNewWindow(link)}
  style="transform: translateY({-$hoverAnimation}px);"
>
  <i class={i_class}></i>
</div>
