<template>
    <div class="container">
        <h1>Users</h1>
        <a href="/">Home</a>
        <hr>
        <div class="input-group">
            <input class="form-control" v-model="val" type="text">
            <button class="btn btn-primary" @clicl="onInput">Load user</button>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                val: ''
            }
        },
        methods: {
            onInput() {
                this.val
            }
        }
    }
</script>
