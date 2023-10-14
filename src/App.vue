<script setup>
import { ref } from 'vue'

const brgy = ref ('')

</script>

<template>
    <div class="form">
        <select v-model="brgy">
            <option value="" disabled>Choose from Options</option>
            <option value="1">Zone 2</option>
            <option value="2">Santa Remedios</option>
            <option value="3">Butag</option>
        </select>
        <p v-if="brgy == '1'">Sabang Park</p>
        <p v-else-if="brgy == '2'">Bariis</p>
        <p v-else-if="brgy == '3'">Kapihan sa Bulod</p>
    </div>

</template>

<style>
.form {
    position: absolute;
    top: 20%;
    left: 20%;
}
</style>