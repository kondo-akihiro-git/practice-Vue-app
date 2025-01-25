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
                console.log(data);
            })
            .catch(error => {
                console.error('Error fetching JSON:', error);
            });

    }
};
</script>