<template>
  <header>
    <div class="container">
      <!-- HEADER LEFT LOGO -->
      <div class="left">
        <img src="../assets/dc-logo.png" alt="" />
      </div>
      <!-- HEADER RIGHT LOGO -->
      <div class="right">
        <ul class="list-item">
          <li v-for="(link, index) in links.nav" :key="index">
            <a
              href="#"
              @click="addClass(index)"
              :class="{ active: links.active == true }"
              >{{ link }}</a
            >
          </li>
        </ul>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: {
        nav: [
          "CHARACTERS",
          "COMICS",
          "MOVIES",
          "TV",
          "GAMES",
          "COLLECTIBLES",
          "VIDEOS",
          "FANS",
          "NEWS",
          "SHOP",
        ],
        active: false,
      },
    };
  },
  methods: {
    addClass(index) {
      if (this.links.active == false) {
        this.links.active = true;
        console.log(this.links.nav[index]);
      } else {
        this.links.active = false;
      }
    },
  },
};
</script>

<style scoped>
header .container {
  display: flex;
  align-items: center;
  max-width: 1200px;
  margin: auto;
}
/* HEADER LEFT */
.left {
  width: 50%;
  padding: 10px 20px;
}

.left img {
  width: 80px;
}

/* HEADER RIGHT */

.right {
  width: 50%;
}

.list-item {
  display: flex;
  justify-content: space-between;
  width: 450px;
  max-width: 100%;
}

.list-item li {
  font-size: 10px;
  display: flex;
}

.list-item a {
  color: #000;
}
a.no-active {
  color: orange;
}
a.active {
  color: blueviolet;
}
</style>
