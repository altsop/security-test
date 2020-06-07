<template>
    <div>
        <button @click="getBoobs">
            Log in
        </button>
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
                    url: '/default-message',
                    headers: {
                        "Authorization": "Basic YWRtaW46YWRtaW4="
                    },
                    responseType: 'json'
                })
            }
        }
    }
</script>
