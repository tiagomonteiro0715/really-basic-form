<template>
  <div>
    <form>
      <label for="name">Name </label>
      <input v-model="name" type="text" />
      <br><br>

      <label for="age">Age </label>
      <input v-model="age" type="text" />
      <br><br>

      <label for="email">Email </label>
      <input v-model="email" type="email" />
      <br><br>

      <label for="phoneNumber">Phone number </label>
      <input v-model="phoneNumber" type="text" />
      <br><br>

      <label for="password">Password </label>
      <input type="password" v-model="password" />
      <br><br>

      <label for="confirmPassword">Confirm Password </label>
      <input type="confirmPassword" v-model="confirmPassword" />
      <br><br>

      <p>Name: {{ name }}</p>
      <p>Age: {{ age }}</p>
      <p>Email: {{ email }}</p>
      <p>PhoneNumber: {{ phoneNumber.split(/(\d{3})/).join(" ") }}</p>
      <p>Password: {{ password }}</p>
      <p>confirmPassword: {{ confirmPassword }}</p>
      <br><br><br><br>

      <p>PasswordSize: {{password.length}}</p>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'Joe Exotic',
      age: '19',
      email: 'tca.monteiro@campus.fct.unl.pt',
      phoneNumber: '918038828',
      password: '',
      confirmPassword: ''

    }
  }
}
</script>

 

 