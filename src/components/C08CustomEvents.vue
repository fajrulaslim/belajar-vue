<template>
    <p>Kirim Data dari Child Component ke Parent Component</p>
    <button @click="sendText">Kirim Data</button>
</template>

<script>
export default {
    name: 'C08CustomEvents',
    data() {
        return {
            txt: "Data dari child component berhasil dikirim."
        }
    },
    methods: {
        sendText() {
            this.$emit("sendTxt", this.txt)
        }
    },
    emits: ["sendTxt"]
}
</script>