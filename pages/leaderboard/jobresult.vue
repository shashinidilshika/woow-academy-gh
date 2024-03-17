<script setup lang="ts">
definePageMeta({
  layout: 'user',
})
</script>

<template>
  <div>
    <main class="flex flex-col justify-center">
      <div id="header">
        <h1>TOP RESUMES</h1>
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
            <td class="level">Adavance Level</td>
            <td class="email">abhi88@gmail.com</td>
          </tr>
          <tr>
            <td class="number">2</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic2.png" alt="Profile Picture" />
            </td>
            <td class="name">Ishara Devindi</td>
            <td class="level">Adavance Level</td>
            <td class="email">ishara123@gmail.com</td>
          </tr>
          <tr>
            <td class="number">3</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic3.jpg" alt="Profile Picture" />
            </td>
            <td class="name">Sanuja Fernando</td>
            <td class="level">Adavance Level</td>
            <td class="email">sanuja@gmail.com</td>
          </tr>
          <tr>
            <td class="number">4</td>
            <td class="img">
              <img class="pic" src="~/assets/images/pic4.png" alt="Profile Picture" />
            </td>
            <td class="name">Sadun Pathirana</td>
            <td class="level">Adavance Level</td>
            <td class="email">sadun99@gmail.com</td>
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
  margin-top: 70px;
  color: #141a39;
  text-transform: uppercase;
  cursor: default;
}

#leaderboard {
  width: 70%;
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

.level {
  font-weight: bold;
  font-size: 1rem;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}
.email {
  text-align: left;
  font-size: 1rem;
}
.points:first-child {
  width: 10rem;
}

.ribbon {
  width: 65rem;
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
