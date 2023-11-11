<template>
    <h3>{{ counter }}</h3>
    <button class="counter-btn" @click="addCounter">
        Increment
    </button>
</template>

<script lang="ts">
import { defineComponent, Ref, ref } from 'vue';
export default defineComponent({
    name: 'CounterComposition',
    setup() {

        let counter: Ref = ref(0);
        const addCounter = (): void => {
            counter.value++;
        }
        return { counter, addCounter }
    }
})
</script>

<style scope>
.counter-btn {
    padding: 15px;
    border: 0;
    outline: 0;
    border-radius: 10px;
    background-color: slategrey;
    color: whitesmoke;
    font-weight: 900;
    cursor: pointer;
}

.counter-btn:hover {
    background-color: rgb(99, 98, 98);
    color: silver;
}
</style>