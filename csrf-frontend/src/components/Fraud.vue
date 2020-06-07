<template>
    <div>
        <a href="http://localhost:8080/messsage/default-message">
            Free Icecream
        </a>
    </div>
</template>

<script>

    import axios from 'axios';

    export default {
        name: "Fraud",
        methods: {
            async getBoobs() {
                // const response = await axios.get('http://localhost:8080/messsage/default-message');
                // console.log(response.data)
                axios({
                    method: 'get',
                    url: 'http://localhost:8080/messsage/default-message',
                })
            }
        }
    }
</script>
