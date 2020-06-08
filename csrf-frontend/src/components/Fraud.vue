<template>
    <div>
        <a href="http://localhost:8080/messsage/default-message">
            Free Ice Cream
        </a>
        <br>
        <button @click="getBoobs">Free Ice Cream</button>
        <br>
        <form action="http://localhost:8080/messsage/default-message">
            <button type="submit">
                Submit Button
            </button>
        </form>
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
                    withCredentials: true
                })
            }
        }
    }
</script>
