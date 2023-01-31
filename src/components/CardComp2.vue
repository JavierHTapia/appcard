<template lang="">
    <div>
        <div class="card" style="width: 16rem;">

            <div class="card-body">
                <h1 class="card-title">{{counter}}</h1>
                <p class="card-text"><strong>Uso de COMPOSITION.API</strong></p>
                <p class="card-text">Incrementa en 1 en cada clic del botón.</p>
                <div class="d-grid gap-2 col-6 mx-auto">
                    <button type="button" class="btn btn-danger btn-sm"   @click="addCounter" >Incrementar</button>
                    <button type="button" class="btn btn-warning btn-sm"  @click="subsCounter">Decrementar</button>
                    <button type="button" class="btn btn-success btn-sm"  @click="resetCounter">Reset</button>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import {defineComponent,ref} from 'vue'
export default defineComponent({
    name:'CardComp2',
    setup(){
        let counter = ref(0);
        const addCounter = () => {
            counter.value++
        }
        const subsCounter =()=>{
            counter.value--
        }
        const resetCounter =()=>{
            counter.value = 0
        }        
        return {counter,addCounter,subsCounter,resetCounter}
    }
})
</script>
<style scope>
    .card-title{
        font-size: 100px;
        font-weight: 800;
        color: rgb(77, 19, 133);
    }
</style>