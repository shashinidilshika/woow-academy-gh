<script setup lang="ts">
import { ref } from 'vue'

const formData = ref({
  companyName: '',
  jobTitle: '',
  role: '',
  minExperience: null,
  jobDescription: '',
  requiredQualifications: '',
  requiredSkills: '',
  salary: null,
  location: '',
  country: '',
  workType: '',
  preference: '',
  responsibilities: '',
})

const submitForm = (): void => {
  // Handle form submission logic here
  console.log(formData.value)
}
</script>

<template>
  <div class="form-container">
    <div >
      <h2>Do you want to filter </h2>
      <h2>suitable candidates for your</h2>
      <h2>job requirements</h2>
      <h2>among our learners?</h2>
      <br /><br />
      <p></p>
      <img class="header-image" src="~/assets/images/j1.png" alt="job page" />
    </div>

    <div class="background">
      <form @submit.prevent="submitForm" class="form">

        <div class="form-group">
          <label for="jobTitle">Job Title</label>
          <input id="jobTitle" type="text" v-model="formData.jobTitle" required />
        </div>

        <div class="form-group">
          <label for="jobDescription">Job Description</label>
          <textarea id="jobDescription" v-model="formData.jobDescription" required></textarea>
        </div>

        <div class="form-group">
          <div class="flex-row">
            <div class="flex-col">
              <label for="minExperience">Minimum Experience</label>
              <input id="minExperience" type="number" v-model="formData.minExperience" required />
            </div>
            <div class="flex-col">
              <label for="salary">Salary</label>
              <input id="salary" type="number" v-model="formData.salary" required />
            </div>
          </div>
        </div>

        <div class="form-group">
          <div class="flex-row">
            <div class="flex-col">
              <label for="location">Location</label>
              <input id="location" type="text" v-model="formData.location" required />
            </div>
            <div class="flex-col">
              <label for="country">Country</label>
              <input id="country" type="text" v-model="formData.country" required />
            </div>
          </div>
        </div>

        <div class="form-group flex-row">
          <div class="flex-col">
            <label for="workType">Work Type</label>
            <select id="workType" v-model="formData.workType" required>
              <option value="Intern">Intern</option>
              <option value="Temporary">Temporary</option>
              <option value="Full-Time">Full-Time</option>
              <option value="Contract">Contract</option>
              <option value="Part-Time">Part-Time</option>
            </select>
          </div>
          <div class="flex-col">
            <label for="preference">Preference</label>
            <select id="preference" v-model="formData.preference" required>
              <option value="Female">Female</option>
              <option value="Male">Male</option>
              <option value="Both">Both</option>
            </select>
          </div>
        </div>

        <div class="form-group">
          <label for="requiredQualifications">Required Qualifications</label>
          <textarea id="requiredQualifications" v-model="formData.requiredQualifications" required></textarea>
        </div>

        <div class="form-group">
          <label for="requiredSkills">Required Skills</label>
          <textarea id="requiredSkills" v-model="formData.requiredSkills" required></textarea>
        </div>
        
        <NuxtLink to="/leaderboard/jobresult">
        <div class="button-container">
          <button type="submit">Submit</button>
        </div>
      </NuxtLink>
      </form>
    </div>
  </div>
</template>

<style scoped>
.form-container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 140vh;
  background: linear-gradient(246.75deg, rgba(109, 132, 214, 0.671) 50.99%, #010c30dc);
}

h2 {
  color: #f2f2f5;
  font-size: 40px;
  font-weight: bold;
  font-family: 'Rubik', sans-serif;
  font-display: left;
  padding-right: 40px;
}

.header-image {
  max-width: 100%;
  height: auto;
  margin-top: 20px;
  padding-right: 70px;
}

.background {
  background-color: #4d4a4acb;
  border-radius: 30px;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.form {
  max-width: 600px;
  width: 100%;
  background-color: #c2c6c99a;
  padding: 30px;
  border-radius: 30px;
  box-shadow: 0 0 20px rgba(36, 35, 35, 0.1);
}
.form-group {
  margin-bottom: 20px;
}
label {
  display: block;
  margin-bottom: 2px;
}
input[type='text'],
input[type='number'],
select,
textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 4px;
  box-sizing: border-box;
  margin-top: 3px;
  margin-bottom: 10px;
  resize: vertical;
  font-size: 16px;
}
.flex-row {
  display: flex;
  gap: 20px;
}
.flex-col {
  flex: 1;
}

.button-container {
  text-align: center;
}

button[type='submit'] {
  background-color: #007bff;
  color: white;
  padding: 12px 50px;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-size: 16px;
}
button[type='submit']:hover {
  background-color: #0056b3;
}
</style>
