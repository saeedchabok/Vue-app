<template>
    <div>
        <h1>{{ name }}</h1>
        <p>{{ nr }}</p>
        <p v-if='gender'>man</p>
        <p v-else>woman</p>
        <p v-for="customer in customers" :key="customer.id">
 {{ customer.name }}, {{ customer.city }}</p>
    </div>



</template>

<script>
export default {
    name: 'App',
    components:
        {},
    data: () => ({
        name: 'Saeed',
        nr: 1,
        gender: true,
        customers:
            [
                { id: 1, name: 'ali', city: 'berlin' },
                { id: 2, name: 'max', city: 'bremen' }
            ]
    })
}
</script>

<style  scoped>

</style>