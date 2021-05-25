<template>
    <div class="name-list">
        <div 
            :key="name.id"
            v-for="name in names"
        >
            <Name :name="name"/>
        </div>
    </div>
</template>

<script>
import Name from './Name';

export default {
    name: 'NameList',
    components: {
        Name
    },
    props: {
         names: Array
    }
}
</script>

<style scoped>

.name-list {
    padding: 0.5rem 1rem;
}

</style>