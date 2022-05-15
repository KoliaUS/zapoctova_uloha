<script setup>
import TheWelcome from '@/components/TheWelcome.vue';

export default {
  components: {TheWelcome},
data() {
  return {
    books: []
  }
},
async created() {
  const res = await fetch('http://localhost:3000/books',{method:'GET'});
  console.log(res);
  this.articles = await res.json();
}
}


</script>

<template>
  <main>
    <section class="py-5 text-center container">
      <div class="row py-lg-5">
        <div class="col-lg-6 col-md-8 mx-auto" v-for="book in books">
         <preview :id="book.id" :name="book.name" :autor="book.autor" :about="book.about" :count="book.count"></preview>
          <p>
            <a href="#" class="btn btn-primary my-2">Main call to action</a>
            <a href="#" class="btn btn-secondary my-2">Secondary action</a>
          </p>
        </div>
      </div>
    </section>
  </main>
</template>


