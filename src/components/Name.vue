<template>
    <div class="name-item">
        <div>
            <div class="name-text">{{ `${name.fullName}` }}</div>
            <div class="name-text">{{ `(${name.nihongo})` }}</div>
        </div>
        <div>
            <Button 
                text="編集" 
                color="blue"
                width="70px"
            />
            <Button 
                text="削除" 
                color="red"
                width="70px"
            />
        </div>
    </div>
</template>

<script>
import Button from './Button';

export default {
    name: 'Name',
    props: {
         name: Object
    },
    components: {
        Button
    }
}
</script>

<style scoped>

.name-item {
    background-color: #f0e8e8;
    margin: 0.5rem 0;
    padding: 1rem;
    border-radius: 5px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.name-text {
    font-size: 20px;
    flex: 1;
}

</style>