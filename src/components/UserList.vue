<!--<template>
  <table>
    <thead>
      <tr>
        <th>#</th>
        <th>Name</th>
        <th>2name</th>
        <th>Active</th>
        <th>Balance</th>
        <th>email</th>
        <th>telephone</th>
        <th>Registration</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="item in users" :key="item.id">
        <td>{{ item.id }}</td>
        <td>{{ item.firstName }}</td>
        <td>{{ item.email }}</td>
      </tr>
    </tbody>
  </table>
</template>-->

<template>
<div>
  <div v-for="item in users" :key="item.id">
    <div>
      {{item.id}}
    </div>
  </div>
</div>
</template>


<script>
export default {
  name: "UserList",
  props: {
    users: {
      type: Array,
      required: true
    }
  }
};
</script>
