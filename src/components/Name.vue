<template>
    <div class="name-item">
        <div>
            <div class="name-text">{{ `${name.title}` }}</div>
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
    background-color: #FFF;
    margin: 1rem 0;
    padding: 1rem;
    border-radius: 5px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    box-shadow: -1px 1px 6px 3px rgba(164,156,156,1);
    -webkit-box-shadow: -1px 1px 6px 3px rgba(164,156,156,1);
    -moz-box-shadow: -1px 1px 6px 3px rgba(164,156,156,1);
}

.name-text {
    font-size: 20px;
    flex: 1;
}

</style>