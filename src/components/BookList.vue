<template>
    <div>
        <h1> {{ title}}</h1>
        <ul>
            <li v-for="book in books">{{book.title}}:{{book.author}}</li>
        </ul>
    </div>
</template>
<script>
export default {
    name: 'BookList',
    data(){
        return {
            title: 'All Books',
            books: [
                {title: 'Tung', author: 'Tung test'},
                {title: 'Tung2', author: 'Tung test2'},
                {title: 'Tung3', author: 'Tung test3'},
            ]

        }
    }
}
</script>

<style>
h1, h2 {
   font-weight: normal 
}
ul{
    list-style-type: none;
    padding: 0;
}
li{
    display: block;
    margin: 0 10px;
}
</style>