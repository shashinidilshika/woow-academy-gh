<script setup lang="ts">
import { ref } from 'vue'

definePageMeta({
  layout: 'user',
})

const searchQuery = ref('')

const search = (): void => {
  // Handle the search logic here based on the value in searchQuery
  console.log('Search Query:', searchQuery.value)
  // You can perform additional actions here, such as filtering data or making API requests
}
</script>

<template>
  <div>
    <main class="flex flex-col justify-center">
      <img class="IMAGE" src="~/assets/images/python1.jpeg" />
      <img class="IMAGE-2" src="~/assets/images/C++.webp" />
      <img class="IMAGE-3" src="~/assets/images/java.jpg" />
      <img class="IMAGE-4" src="~/assets/images/cr-c.png" />
      <img class="IMAGE-5" src="~/assets/images/IMAGE.png" />
      <img class="IMAGE-6" src="~/assets/images/c.png" />
      <img class="IMAGE-7" src="~/assets/images/python2.png" />
      <img class="IMAGE-8" src="~/assets/images/python3.png" />
      <img class="IMAGE-9" src="~/assets/images/crs1.png" />
      <img class="IMAGE-10" src="~/assets/images/crs2.png" />
      <img class="IMAGE-11" src="~/assets/images/sql.png" />
      <img class="IMAGE-12" src="~/assets/images/crs3.png" />
      <img class="IMAGE-13" src="~/assets/images/crs4.png" />
      <img class="IMAGE-14" src="~/assets/images/python.png" />
      <img class="IMAGE-15" src="~/assets/images/r.png" />
      <img class="IMAGE-16" src="~/assets/images/html.png" />
      <img class="IMAGE-17" src="~/assets/images/css.png" />
      <img class="IMAGE-18" src="~/assets/images/php.png" />
      <img class="IMAGE-19" src="~/assets/images/jquery.jpg" />
      <img class="IMAGE-20" src="~/assets/images/crs5.png" />
      <img class="IMAGE-21" src="~/assets/images/react.webp" />
      <img class="IMAGE-22" src="~/assets/images/crs6.png" />
      <img class="IMAGE-23" src="~/assets/images/crs7.png" />
      <img class="IMAGE-24" src="~/assets/images/crs8.png" />
      <img class="IMAGE-25" src="~/assets/images/crs9.png" />
      <img class="IMAGE-26" src="~/assets/images/crs10.png" />
      <img class="IMAGE-27" src="~/assets/images/crs11.png" />
      <img class="IMAGE-28" src="~/assets/images/crs12.png" />

      <div id="header">
        <h1>TOP LEARNERS</h1>
      </div>

      <!-- Search Input and Button & Job Requirement Button -->
      <div id="search-container">
        <NuxtLink to="/leaderboard/job">
          <button class="job-requirement-button">Job Requirement</button>
        </NuxtLink>
        <input v-model="searchQuery" type="text" placeholder="Search your Name..." class="search-input" />
        <button class="search-button" @click="search">Search</button>
      </div>

      <!-- Leaderboard Table -->
      <div id="leaderboard">
        <div class="ribbon"></div>
        <table>
          <tr>
            <td class="number">1</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic1.jpg" alt="Profile Picture" />
            </td>
            <td class="name">Abhi Senanayaka</td>
            <td class="points">
              258             
              <img
                class="gold-medal"
                src="https://github.com/malunaridev/Challenges-iCodeThis/blob/master/4-leaderboard/assets/gold-medal.png?raw=true"
                alt="gold medal"
              />
            </td>
          </tr>
          <tr>
            <td class="number">2</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic2.png" alt="Profile Picture" />
            </td>
            <td class="name">Ishara Devindi</td>
            <td class="points">253</td>
          </tr>
          <tr>
            <td class="number">3</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic3.jpg" alt="Profile Picture" />
            </td>
            <td class="name">Sanuja Fernando</td>
            <td class="points">213</td>
          </tr>
          <tr>
            <td class="number">4</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic4.png" alt="Profile Picture" />
            </td>
            <td class="name">Gonzalo da Cruz</td>
            <td class="points">210</td>
          </tr>
          <tr>
            <td class="number">5</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic5.jpg" alt="Profile Picture" />
            </td>
            <td class="name">Kasun Madhusanka</td>
            <td class="points">195</td>
          </tr>
          <tr>
            <td class="number">6</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic6.jpg" alt="Profile Picture" />
            </td>
            <td class="name">Ryne C Allen</td>
            <td class="points">190</td>
          </tr>
          <tr>
            <td class="number">7</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic7.jpeg" alt="Profile Picture" />
            </td>
            <td class="name">Pavel Patrin</td>
            <td class="points">187</td>
          </tr>
          <tr>
            <td class="number">8</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic8.jpg" alt="Profile Picture" />
            </td>
            <td class="name">Tharusha Udawatta</td>
            <td class="points">172</td>
          </tr>
          <tr>
            <td class="number">9</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic9.png" alt="Profile Picture" />
            </td>
            <td class="name">Shenal Illeperuma</td>
            <td class="points">170</td>
          </tr>
          <tr>
            <td class="number">10</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic10.jpg" alt="Profile Picture" />
            </td>
            <td class="name">Jaivrat Das</td>
            <td class="points">165</td>
          </tr>
        </table>
      </div>
    </main>
  </div>
</template>

<style scoped>
* {
  font-size: 62, 5%;
  box-sizing: border-box;
  margin: 0;
}

body {
  height: 100%;
  width: 100vh;
  min-height: 100vh;
  background-color: #fbfaff;
  display: flex;
  align-items: center;
  justify-content: center;
}

main {
  width: 100%;
  height: 100%;
  background-color: #ffffff;
  -webkit-box-shadow: 0px 5px 15px 8px #e4e7fb;
  box-shadow: 0px 5px 15px 8px #e4e7fb;
  display: flex;
  flex-direction: column;
  align-items: center;
  border-radius: 0.5rem;
  justify-content: center;
}

#header {
  width: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 2.5rem 2rem;
}

h1 {
  font-family: 'Rubik', sans-serif;
  font-size: 3.5rem;
  font-weight: 700;
  margin-top: 160px;
  color: #141a39;
  text-transform: uppercase;
  cursor: default;
}

#leaderboard {
  width: 60%;
  position: relative;
}

table {
  width: 100%;
  border-collapse: collapse;
  table-layout: fixed;
  color: #141a39;
  cursor: default;
}

tr {
  transition: all 0.2s ease-in-out;
  border-radius: 0.2rem;
}

tr:not(:first-child):hover {
  background-color: #fff;
  transform: scale(1.1);
  -webkit-box-shadow: 0px 5px 15px 8px #e4e7fb;
  box-shadow: 0px 5px 15px 8px #e4e7fb;
}

tr:nth-child(odd) {
  background-color: #f9f9f9;
}

tr:nth-child(1) {
  color: #fff;
}

td {
  height: 5rem;
  font-family: 'Rubik', sans-serif;
  font-size: 1.4rem;
  padding: 1rem 2rem;
  position: relative;
}

.number {
  width: 1rem;
  font-size: 2.2rem;
  font-weight: bold;
  text-align: left;
}

.pic {
  width: 65px;
  height: 65px;
  top: 4.5px;
  left: 75px;
  position: absolute;
  object-fit: cover;
}

.name {
  text-align: left;
  font-size: 1.2rem;
}

.points {
  font-weight: bold;
  font-size: 1.3rem;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

.points:first-child {
  width: 10rem;
}

.gold-medal {
  height: 3rem;
  margin-left: 1.5rem;
}

.ribbon {
  width: 53rem;
  height: 5.5rem;
  top: -0.5rem;
  background-color: #4d4bd6af;
  position: absolute;
  left: -1rem;
  -webkit-box-shadow: 0px 15px 11px -6px #7a7a7d;
  box-shadow: 0px 15px 11px -6px #7a7a7d;
}

.ribbon::before {
  content: '';
  height: 1.5rem;
  width: 1.5rem;
  bottom: -0.8rem;
  left: 0.35rem;
  transform: rotate(45deg);
  background-color: #5c5be5;
  position: absolute;
  z-index: -1;
}

.ribbon::after {
  content: '';
  height: 1.5rem;
  width: 1.5rem;
  bottom: -0.8rem;
  right: 0.35rem;
  transform: rotate(45deg);
  background-color: #5c5be5;
  position: absolute;
  z-index: -1;
}

#search-container {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: flex-end;
  margin: 20px 0;
  margin-right: 180px;
}

.search-input {
  padding: 10px;
  font-size: 15px;
  margin-right: 10px;
  width: 320px;
  background: rgba(232, 239, 245, 0.63);
}

.search-button {
  padding: 10px 20px;
  font-size: 16px;
  text-transform: uppercase;
  background-color: #5c5be5;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.search-button:hover {
  background-color: #3838b8;
}

.job-requirement-button {
  margin-right: 500px;
  margin-left: 80px;
  padding: 10px 33px;
  font-size: 16px;
  text-transform: uppercase;
  background-color: #5c5be5;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.IMAGE {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 176px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-2 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 231px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-3 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 286px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-4 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 341px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-5 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 396px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-6 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 451px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-7 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 506px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-8 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 561px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-9 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 616px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-10 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 671px;
  position: absolute;
  object-fit: cover;
}
.IMAGE-11 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 726px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-12 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 781px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-13 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 836px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-14 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 891px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-15 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 946px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-16 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 1001px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-17 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 1056px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-18 {
  width: 43px;
  height: 43px;
  top: 50px;
  left: 1111px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-19 {
  width: 43px;
  height: 43px;
  top: 105px;
  left: 396px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-20 {
  width: 43px;
  height: 43px;
  top: 105px;
  left: 451px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-21 {
  width: 43px;
  height: 43px;
  top: 105px;
  left: 506px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-22 {
  width: 43px;
  height: 43px;
  top: 105px;
  left: 561px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-23 {
  width: 43px;
  height: 43px;;
  top: 105px;
  left: 616px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-24 {
  width: 43px;
  height: 43px;
  top: 105px;
  left: 671px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-25 {
  width: 43px;
  height: 43px;
  top: 105px;
  left: 726px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-26 {
  width: 43px;
  height: 43px;
  top: 105px;
  left: 781px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-27 {
  width: 43px;
  height: 43px;
  top: 105px;
  left: 836px;
  position: absolute;
  object-fit: cover;
}

.IMAGE-28 {
  width: 43px;
  height: 43px;
  top: 105px;
  left: 891px;
  position: absolute;
  object-fit: cover;
}

@media (max-width: 740px) {
  * {
    font-size: 70%;
  }
}

@media (max-width: 500px) {
  * {
    font-size: 55%;
  }
}

@media (max-width: 390px) {
  * {
    font-size: 45%;
  }
}
</style>
