<template>
  <div class="wrapper">
    <div class="main-container">
      <div class="container-one">
        <div>
          <img src="../assets/huda.jpeg" alt="" class="hudaImg" />
          <h3>Huda Sabagh</h3>
          <p>Frontend Developer</p>
        </div>
        <div class="socialMedia">
          <div class="link">
            <a href=""><h2>Github</h2></a>
            <i class="fa-brands fa-github"></i>
          </div>

          <div class="link">
            <a href=""><h2>LinkedIn</h2></a>
            <i class="fa-brands fa-linkedin"></i>
          </div>

          <div class="link">
            <a href=""><h2>Facebook</h2></a>
            <i class="fa-brands fa-facebook"></i>
          </div>
        </div>
      </div>
      <div class="container-two">
        <div class="about-me">
          <h1>About me</h1>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Ratione
            eligendi aliquam officiis vitae ipsa dolores est quia neque corrupti
            beatae! Iure saepe id odio, cumque explicabo totam qui quis
            architecto expedita libero laudantium molestias quae deserunt eaque
            quas, ut nostrum enim quasi. Quos quibusdam minima illum accusantium
            dignissimos illo a! Lorem ipsum dolor, sit amet consectetur
            adipisicing elit. Deserunt quasi expedita impedit quia iure optio
            dolor vitae magnam totam, earum sit sapiente. Sit possimus, laborum
            velit animi quos ullam nostrum.
          </p>
        </div>
        <div class="skills">
          <h1>Technologies Studied</h1>
          <div class="logs">
            <img src="../assets/html-svgrepo-com.svg" alt="" /><img
              src="../assets/css-svgrepo-com.svg"
              alt=""
            /><img src="../assets/js-svgrepo-com.svg" alt="" /><img
              src="../assets/logo.png"
              alt=""
            /><img src="../assets/node-svgrepo-com.svg" alt="" />
            <img src="../assets/excel-svgrepo-com.svg" alt="" /><img
              src="../assets/adobe-xd-1-logo-svgrepo-com.svg"
              alt=""
            />
            <img
              src="../assets/adobe-illustrator-cc-logo-svgrepo-com.svg"
              alt=""
            /><img
              src="../assets/adobe-photoshop-cs6-logo-svgrepo-com.svg"
              alt=""
            />
          </div>
        </div>
        <div class="project-section">
          <div class="myprojects">
            <a href="">My Projects</a>
          </div>
          <div class="myprojects">
            <a href="">My Resume</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Portfolio",
};
</script>
<style scoped>
.hudaImg {
  border-radius: 50%;

  height: 8rem;
}
.wrapper {
  width: 70%;
  margin: auto;
}
.main-container {
  display: flex;
  flex-direction: row;

  justify-content: center;
  align-content: center;
  padding: 2rem;
  border-radius: 25px;
}
.logs img {
  width: 60px;
  height: 60px;
  margin: 7px;
  transform: perspective(750px) translate3d(0px, 0px, -250px) rotateX(27deg)
    scale(0.9, 0.9);
  border-radius: 20px;
  box-shadow: 0 70px 40px -20px rgba(0, 0, 0, 0.2);
  transition: 0.4s ease-in-out transform;
}
.logs img:hover {
  transform: translate3d(0px, 0px, -250px);
}
.link a {
  text-decoration: none;
  color: #d7c29eff;
  font-size: 12px;
}
.link i {
  font-size: 2rem;
  margin-bottom: 5px;
}
.link:nth-child(1),
.link:nth-child(2) {
  border-bottom: 1px solid #d7c29eff;
}
.container-one {
  color: #d7c29eff;
  padding: 2.5%;
  width: 30%;
  background: #343148ff;
  border-radius: 50px 0px 0px 50px;
}
.container-two {
  width: 70%;
  padding: 2.5%;
  background-color: #d7c29eff;

  border-radius: 0px 50px 50px 0px;
}
.about-me {
  text-align: left;
}
.project-section {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 20px;
}
.myprojects {
  background-color: #343148ff;
  padding: 20px;
  transform: perspective(1500px) rotateY(15deg);
  border-radius: 1rem;
  box-shadow: rgba(0, 0, 0, 0.4) 0px 25px 50px -12px;
  transition: transform 1s ease 0s;
}
.myprojects:hover {
  background: rgba(52, 49, 72, 0.9);
  transform: perspective(3000px) rotateY(5deg);
}
.myprojects a {
  text-decoration: none;
  color: #d7c29eff;
  font-weight: 600;
}
.socialMedia {
  margin-top: 40px;
}
@media only screen and (max-width: 850px) {
  .wrapper {
    width: 100%;
  }
}
</style>
