<template>
    <div class="">
        <table class="table table-dark">
            <thead>
            <tr>
                <th scope="col">#</th>
                <th scope="col">Titulo</th>
                <th scope="col">Body</th>
            </tr>
            </thead>
            <tbody>
            <tr v-for="post in posts" :key="post.id">

                <td>{{post.id}}</td>
                <td>{{post.titulo}}</td>
                <td>@{{post.body}}</td>
            </tr>

            </tbody>
        </table>
    </div>
</template>

<script>
    export default {
        name: "Posts",
        data(){
            return{
                posts:[
                    {id:1,titulo:'Post 1',body:'Body 11'},
                    {id:2,titulo:'Post 2',body:'Body 22'}
                ]
            }
        }
    }
</script>

<style scoped>

</style>