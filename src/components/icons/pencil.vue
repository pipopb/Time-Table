<template>
    <svg 
        :width="width"
        :height="height"
        aria-labelledby="Editar"
        role="img"
        viewBox="0 0 24 24"
        xmlns="http://www.w3.org/2000/svg">
                
        <g :fill="color"> <slot/> </g>
        
        <title>
            Editar
        </title>
        <path d="M14.078 7.061l2.861 2.862-10.799 10.798-3.584.723.724-3.585 10.798-10.798zm0-2.829l-12.64 12.64-1.438 7.128 7.127-1.438 12.642-12.64-5.691-5.69zm7.105 4.277l2.817-2.82-5.691-5.689-2.816 2.817 5.69 5.692z"/>
    </svg>
</template>

<script>
export default {
    name: 'Pencil',
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
            default: 'white'
        }
    }
}
</script>