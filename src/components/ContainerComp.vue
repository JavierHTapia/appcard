<template lang="">

        <div class="container-comp">
            <div class="row">
                <div class="col-2">
                    <div class="container-list"><ListComp></ListComp></div>
                </div>
                <div class="col-10">
                    <div class="container-main"><CardComp></CardComp></div>
                </div>
            </div>
        </div>

</template>
<script>
import ListComp from '../components/ListComp.vue'
import CardComp from '../components/CardComp.vue'

export default {
  name: 'ContainerComp',
  components: {
    ListComp,CardComp
  }
}
</script>
<style scope>
    .container-comp{
        background-color: bisque;
    }
    .container-main{
        padding: 15px;
    }
    .container-list{
        padding-top: 15px;
    }    
</style>