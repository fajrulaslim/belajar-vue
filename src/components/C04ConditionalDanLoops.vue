<template>
    <div v-if="skills.length">
        <h3>Skills</h3>
        <ul>
            <li v-for="item in skills" :key="item.id">{{ item.title }}</li>
        </ul>
    </div>
    <div v-else>
        <p>Data not found</p>
    </div>
</template>

<script>
export default {
    name: 'C04ConditionalDanLoops',
    data() {
        return {
            skills: [
                { id: 1, title: "Frontend Engineer" },
                { id: 2, title: "Backend Engineer" },
                { id: 3, title: "Fullstack Engineer" }
            ]
        }
    },
}
</script>