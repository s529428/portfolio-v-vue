<template>
    <svg xmlns="http://www.w3.org/2000/svg"
        :width="width"
        :height="height" 
        viewBox="0 0 433.05 65.58"
    >
        <title
            :id="logo"
            lang="en"
        > {{ iconName }} icon</title>
        <g :fill="iconColor">
        <slot />
        </g>
    </svg>
</template>
<script>
export default {
    props: {
        iconName: {
            type: String,
            default: 'box'
        },
        width: {
            type: [Number, String],
            default: 18
        },
        height: {
        type: [Number, String],
        default: 18
        },
        iconColor: {
        type: String,
        default: 'currentColor'
        }
    }
}
</script>