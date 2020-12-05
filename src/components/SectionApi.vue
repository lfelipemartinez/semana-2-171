<template>
  <div class="container-fluid align-content-center">
      <h2 class="text-center text-info font-weight-bold p-5">Noticias</h2>
      <div class="row align-items-center" >
        <div class="col-md-6 p-5" v-for="(news, index) of news" v-bind:key="index" style="marign-right:1px">
          <div class="row p-3">
                <div class="col-md-6 col-xs-12">
                    <img
                        v-bind:src="news.urlToImage"
                        class="img-fluid rounded"
                        :alt="'noticias' + index"
                    />
                </div>
                <div class="col-md-6">
                    <p class="text-justify text-info font-weight-bold">{{ news.title }}</p>
                    <p class="text-justify"> {{news.description}}</p>
                </div>
          </div>
          <div class="row justify-content-end p-3 border-bottom border-info ">
              <div class="col-md-6">
              <a  v-bind:href="news.url" target="_blank" class="btn btn-outline-info">Leer mas</a>
              </div>
          </div>
        </div>
      
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "SectionApi",
  data() {
    return {
      news: null,
    };
  },
  mounted() {
    axios
      .get(
        "http://newsapi.org/v2/top-headlines?country=co&apiKey=6717cf19c07941c0bf84d47c1c164dc7"
      )
      .then((response) => {
        var articles = response.data.articles;
        this.news = articles.slice(0, 4);
        console.log(articles.slice(0, 4));
      });
  },
};
</script>