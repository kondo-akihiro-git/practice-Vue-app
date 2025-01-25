<template>
    <div>
        <h1>JSON Data</h1>
        <ul>
            <li v-for="(item, index) in jsonData" :key="index">
                {{ item.name }} - {{ item.value }}
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    data() {
        return {
            jsonData: []
        };
    },
    mounted() {
        fetch('/data/sample.json')
            .then(response => response.json())
            .then(data => {
                this.jsonData = data;
            })
            .catch(err => console.error(err));
    }
};
</script>