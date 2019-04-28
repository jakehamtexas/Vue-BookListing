<template>
  <div>
    <h1>{{ title }}</h1>
    <li v-for="book in books">{{book.title}} : {{book.author}}</li>
  </div>
</template>

<script>
export default {
  name: 'BookList',
  data() {
    return {
      title: 'All Books',
      books: 
      [
        {
          title:'The Old Man And The Sea', 
          author: "Some Guy"
        },
        {
          title:'Clean Architecture', 
          author: "Uncle Bob"
        },
        {
          title:'Clean Code', 
          author: "Robert C. Martin"
        }
      ]
    }
  }
}
</script>

<style>
h1, h2 {
  font-weight: normal;
}
li {
  list-style-type: none;
  padding: 0;
  display: block;
  margin: 0 10px;
}
</style>
