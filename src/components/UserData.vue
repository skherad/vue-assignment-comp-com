<template>
    <form @submit.prevent="update">
        <label>Name</label>
        <input type="text" placeholder="Name..." v-model="inputName" />
        <label>Age</label>
        <input type="number" placeholder="Age..." v-model="inputAge" />
        <button>Save Changes</button>
    </form>
</template>

<script>
export default {
    data() {
        return {
            inputName: '',
            inputAge: ''
        }
    },
    methods: {
        update() {
            this.$emit('update-friend', this.inputName, this.inputAge)
            event.target.reset()
        }
    }
}
</script>