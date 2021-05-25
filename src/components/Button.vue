<template>
    <button 
        @click="onBtnClick()"
        :style="{ 
            background: color,
            width: width
        }"
        class="btn"
    >
        {{ text }}
    </button>
</template>

<script>
export default {
    name: 'Button',
    props: ['text', 'color', 'width'],
    methods: {
        onBtnClick() {
            console.log("Btn Click")
        }
    }
}
</script>
