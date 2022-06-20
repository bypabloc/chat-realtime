<template>
    <div>
        Users
        List: 
        <ul>
            <li v-for="user in users">
                {{ user.name }}
            </li>
        </ul>
    </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'Users',
  setup() {
    
    const users = ref([
        { name: 'John' },
        { name: 'Jane' },
        { name: 'Bob' },
    ])
    return {
      users
    }
  }
})
</script>