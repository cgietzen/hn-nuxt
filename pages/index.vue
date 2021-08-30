<template>
<div class="f1">
<ul>
  <li v-for="id in ids" :key="id.id">
    {{id}}
  </li>
</ul>
</div>

</template>

<script>
import {mapState} from "vuex";

export default {
  computed: mapState([
    "users",
    "ids"
  ])
}
</script>
