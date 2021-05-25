<template>
  <header>
        <h1>{{ title }}</h1>
        <Button 
            text="+ 名前"
            color="green"
            width="100px"
        />
  </header>
</template>

<script>
import Button from './Button';

export default {
    name: 'Header',
    props: ['title'],
    components: {
        Button
    }
}
</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-around;
        align-items: center;
        margin: 1rem;
        border-bottom: 1px solid #000;
        padding: 1rem;
    }

    h1 {
        font-size: 35px;
    }
</style>
