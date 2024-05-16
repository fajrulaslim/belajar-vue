<template>
    <p>Lifecycle Hooks</p>
</template>

<script>
export default {
    name: 'C05LifecycleDanHooks',
    data() {
        return {
            products: []
        }
    },
    beforeCreate() {
        console.log('Before Create')
    },
    created() {
        console.log('Created')
        this.products = [
            { id: 1, title: "Product 1" },
            { id: 2, title: "Product 2" },
            { id: 3, title: "Product 3" }
        ]
    },
    beforeMount() {
        console.log('Before Mount')
    },
    mounted() {
        console.log('Mounted')
    }
}
</script>