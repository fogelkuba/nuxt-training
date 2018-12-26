<template>
    <div class="container">
        <h1>Users</h1>
        <a href="/">Home</a>
        <hr>
        <div class="input-group">
            <input name="userId" class="form-control" v-model="userId" type="text">
            <div class="input-group-append">
                <button class="btn btn-outline-secondary" type="button" @click="onInput">Load user</button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                userId: ''
            }
        },
        methods: {
            onInput() {
                this.$router.push(`/users/${this.userId}`)
            }
        }
    }
</script>
