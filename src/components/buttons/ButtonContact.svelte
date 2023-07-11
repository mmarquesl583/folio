<script>
    export let title
    export let icon

    let btn_class = "hover:cursor-pointer w-12 h-12 border rounded-full flex items-center justify-center mr-2 ml-2"
    btn_class += ` btn-${title}`
    icon += ` text-3xl`
</script>

<div  class={btn_class} {title}>
    <i class="{icon}"></i>
</div>

<style>
    .btn-WhatsApp{
        background-color: #52c769;
        color: white
    }
    .btn-WhatsApp:hover{
        background-color: #49b45f
    }
    .btn-Linkedin{
        background-color: #449cf5;
        color: white
    }
    .btn-Linkedin:hover{
        background-color: rgb(45, 131, 218)
    }
    .btn-GitHub{
        background-color: white
    }
    .btn-GitHub:hover{
        background-color: #d1d1d1
    }
    .btn-Email{
        background-color: #ff8d8d;
        color: white
    }
    .btn-Email:hover{
        background-color: #dd7272
    }
    .btn-Instagram{
        background: radial-gradient(circle at 30% 107%, #fdf497 0%, #fdf497 5%, #fd5949 45%, #d6249f 60%, #285AEB 90%);
        color: white;
    }
    .btn-Instagram:hover{
        background: radial-gradient(circle at 30% 107%, #e2d21a 0%, #ffed26 5%, #fa2e1b 45%, #cf0790 60%, #0241ff 90%);

    }
</style>