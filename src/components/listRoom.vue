<template>
    <div>
        <div v-for="item in items" :key="item.id">
            <button></button>{{ item.name }}
        </div>
    </div>
</template>
<script>
export default {
    name: 'listItem',
    props: ['items']
}
</script>
<style scoped>
ul{
    list-style-type: none;
    color: red;
    font-family: 'Orbitron', sans-serif;
    text-shadow: 4px 4px 4px #aaa;
    font-size: 20px;
}
</style>


