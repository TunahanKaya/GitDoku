<template>
  <button @click="addUser($event)">Add User</button>
</template>

<script>
export default {
  methods: {
    addUser(event) {
      event.preventDefault();
      this.$emit(
        'new-user',
        { name: 'Chris', age: 20, showAge: false },
      );
    },
  },
};
</script>

<style lang="scss" scoped>
button {
  margin-left: 1em;
  background-color: yellowgreen;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
}
</style>
