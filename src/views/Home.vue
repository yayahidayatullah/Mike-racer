<template>
  <div>
    <buttons class="button" play="play"/>
    <list :items="listRoom"/>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import buttons from '@/components/button.vue'
import list from '@/components/listRoom.vue'

export default {
  data(){
    return {
      listRoom: [{
        id: 1,
        name: 'balapan sapi'
      },
      {
        id: 2,
        name: 'balap kodok'
      },
      {
        id: 3,
        name: 'nooby room'
      }]
    }
  },
  name: 'home',
  components: {
    buttons,
    list
  }
}
</script>

