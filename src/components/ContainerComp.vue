<template lang="">

        <div class="container-comp">
            <div class="row">
                <div class="col-2">
                    <div class="container-list"><ListComp></ListComp></div>
                </div>
                <div class="col-10">
                    <div class="container-main">
                        <div class="row">
                            <div class="col-4"><CardComp></CardComp></div>
                            <div class="col-4"><CardComp2></CardComp2></div>
                            <div class="col-4"></div>
                         </div>
                    </div>
                </div>
            </div>
        </div>

</template>
<script>
import ListComp from '../components/ListComp.vue'
import CardComp from '../components/CardComp.vue'
import CardComp2 from '../components/CardComp2.vue'

export default {
  name: 'ContainerComp',
  components: {
    ListComp,CardComp,CardComp2
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