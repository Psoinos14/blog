<template>
  <div class="container">
    <h1>New User</h1>
    <form v-on:submit.prevent="createUsers()">
      <ul>
        <li v-for="error in errors">{{ error }}</li>
      </ul>
      Name:
      <input text="text" v-model="newUserName" />
      <input type="submit" value="Create" />
    </form>
  </div>
</template>
