<template>
  <div>
    <div>
      <p>spisok polzovateley</p>
    </div>
    <div v-if="!users.length" class="alert alert-warning">
      loading...
    </div>
    <user-list v-else :users="users" />
  </div>
</template>
<script>
import axios from "axios";
import UserList from "@/components/UserList.vue";

export default {
  name: 'UserList',
  components: {
    UserList
  },
  data :()=>({
    users:[]
  }),
  mounted(){
    this.loadUsers()
  },
  methods:{
    loadUsers(){
      axios.get("http://localhost:3004/users").then(response => {
         this.users = response.data
       })
    }
  }
}
</script>
