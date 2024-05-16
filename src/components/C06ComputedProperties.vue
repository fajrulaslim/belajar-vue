<template>
    <div>
        <input type="text" v-model="cari" placeholder="cari"> <br>
        <ul>
            <li v-for="item in cariData" :key="item.id">{{ item.title }}</li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'C06ComputedProperties',
    data() {
        return {
            cari: "",
            products: [
                { id: 1, title: "Product 1" },
                { id: 2, title: "Product 2" },
                { id: 3, title: "Product 3" }
            ]
        }
    },
    computed: {
        cariData() {
            return this.products.filter((item) => {
                return item.title.match(this.cari)
            })
        }
    }

}
</script>