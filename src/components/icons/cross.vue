<template>
    <svg 
        :width="width"
        :height="height"
        aria-labelledby="Excluir tarefa"
        role="img"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg"
        fill-rule="evenodd"
        clip-rule="evenodd">        
        <g :fill="color"> <slot/> </g>
        
        <title>
            Excluir tarefa
        </title>
        <path d="M12 0c-6.627 0-12 5.373-12 12s5.373 12 12 12 12-5.373 12-12-5.373-12-12-12zm4.151 17.943l-4.143-4.102-4.117 4.159-1.833-1.833 4.104-4.157-4.162-4.119 1.833-1.833 4.155 4.102 4.106-4.16 1.849 1.849-4.1 4.141 4.157 4.104-1.849 1.849z"/>
    </svg>
</template>

<script>
export default {
    name: 'Cross',
    props: {
        width: {
            type: [Number, String],
            default: 24
        },
        height: {
            type: [Number, String],
            default: 24
        },
        color: {
            type: String,
            default: 'black'
        }
    }
}
</script>