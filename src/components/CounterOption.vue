<template>
    <h3>{{ counter }}</h3>
    <button class="counter-btn" @click="addCounter">
        Increment
    </button>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
    name: 'CounterOption',
    // components: {ComponentOne, ComponentTwo}
    data() {
        let counter = 0;
        // Aquí, esta función returna un objeto con todas las variables que vaya a usar el componente.
        return { counter };
    },
    methods: {
        addCounter() {
            this.counter++;
        }
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