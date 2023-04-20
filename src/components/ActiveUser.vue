<template>
    <section>
        <h2>Username: {{ userName }}</h2>
        <h3>Age: {{ userAge }}</h3>
    </section>
</template>

<script>
export default {
    props: {
        userName: {
            type: String,
            required: true
        },
        userAge: {
            type: Number,
            required: true
        }
    },
    methods: {
        
    }
}
</script>