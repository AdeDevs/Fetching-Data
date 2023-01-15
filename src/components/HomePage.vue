<template>
  <div>
    <h2>Data Fetching {{ msg }}</h2>
    <p class="joke">{{ data.joke }}</p>
  </div>
</template>

<script>
export default {
  name: "HomePage",
  props: {
    msg: String,
  },
  data() {
    return {
      data: "",
    };
  },
  mounted() {
    fetch("https://icanhazdadjoke.com/search?term=dog", {
      headers: {
        Accept: "application/json",
      },
    })
      .then((res) => res.json())
      .then((data) => (this.data = data));
  },
};
</script>