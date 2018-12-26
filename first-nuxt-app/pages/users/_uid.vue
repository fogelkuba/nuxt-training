<template>
    <div class="container">
        <h2>Hello user</h2>
        <h3 class="muted"># {{ $route.params.uid }}</h3>
        <a href="/users">Back to Users</a>
    </div>
</template>

<script>
    export default {
        validate (data) {
            console.log('uid: ', data.params.uid);
            // return data.params.uid === '1'
            return /^\d+$/.test(data.params.uid)
            // return true
        }
    }
</script>
