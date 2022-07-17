<template>
  <div class="content">
    <div class="card" v-for="(item, index) in myJson" :key="index">
      <img src="../assets/nils-lindner-drba0TzbCGA-unsplash.jpg" alt="" />
      <div class="container">
        <h3>{{ item.name }}</h3>
        <p>{{ item.descrip }}</p>
        <a :href="item.link1">Show More</a>
      </div>
    </div>
  </div>
</template>
<script>
import myProjectInfo from "/infoPro.json";
export default {
  name: "Card",
  data() {
    return {
      myJson: myProjectInfo,
    };
  },
};
</script>
<style>
.content {
  width: 70%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-content: center;
  flex-wrap: wrap;
  margin: auto;
}
.card {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  transition: 0.3s;
  width: 30%;
  border-radius: 10px;
  margin: 20px;
  height: 300px;
  border-radius: 1rem;
  box-shadow: rgba(0, 0, 0, 0.4) 0px 25px 50px -12px;
  transition: transform 0.5s ease 0s;
  white-space: wrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
}

.container {
  padding: 2px 16px;
}

.card img {
  border-radius: 10px 10px 0 0;
  width: 100%;
  height: 10rem;
}
.container a {
  padding: 10px;
  text-decoration: none;
  color: #343148ff;
  background-color: #d7c29eff;
  margin-bottom: 10px;
  border-radius: 10px;
  transition: 1s ease;
}
.container a:hover {
  background-color: rgba(215, 194, 158, 0.596);
  font-weight: 700;
}
.container p {
  margin-bottom: 20px;
}
@media only screen and (max-width: 850px) {
  .content {
    width: 100%;
  }
  .card {
    font-size: 16px;
    width: 100%;
    height: 50vh;
  }
  .container a {
    margin-bottom: 20px;
  }
}
@media screen and (max-width: 280px) {
  .card {
    font-size: 16px;
    width: 100%;
    height: 60vh;
  }
}
</style>
