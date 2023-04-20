<template>
    <section>
        <active-user :user-name="user.username" :user-age="user.age"></active-user>
        <user-data @update-friend="updateUserInfo"></user-data>
    </section>
</template>

<script>
export default {
    data(){
        return {
            user: {
                username: 'Shahrzad',
                age: 31
            }
        }
    },
    methods: {
        updateUserInfo(newName, newAge){
            this.user.username = newName
            this.user.age = +newAge
        }
    }
}
</script>