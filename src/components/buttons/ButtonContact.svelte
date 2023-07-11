<script>
    export let title = "oi"
    export let color
    export let icon

    let btn_class = "w-12 h-12 border rounded-full border-black "
    btn_class += `bg-${color}`
    icon += ` text-4xl`
</script>

<div  class={btn_class} {title}>
    <i class={icon}></i>
</div>