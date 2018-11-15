<template>
            <ul class="buttons">
                <li><a href="#"><span :title='play'>{{play}}</span></a></li>
            </ul>
</template>
<script>
export default {
    name: 'list',
    props: ['play'] 
}
</script>


