<template>
    <li>
      <span>
        <span class="contact-names">{{ contact.firstName }} {{ contact.lastName }}</span><br> {{ contact.email }}</span>
      <span class="controls">
        <button @click="editContact"><img src="../assets/edit.svg"></button>
      <button @click="deleteContact"><img src="../assets/delete.svg"></button>
      </span>
      
    </li>
  </template>
  
  <script>
  export default {
    props: {
      contact: Object,
    },
    methods: {
      editContact() {
        this.$emit('editContact', this.contact)
      },
      deleteContact() {
        this.$emit('deleteContact', this.contact)
      },
    },
  }
  </script>
  