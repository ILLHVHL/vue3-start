<template>
<div>
  <input type="text" v-model="searchPh" v-bind:placeholder="placeholderText">
  <button type="button" @click="plus()"> + </button>
  <button type="button" @click="minus"> - </button>
  {{ count }}
</div>
</template>

<script>
export default {
  name: "SearchComponent",
  created() { /* 화면이 렌더링 될 때 제일 처음 실행 (1회) */
   // this.createdAlert();
  },
  mounted() { /* 값이 변했을 때 한번 더 실행 = 값이 바뀐 것을 반영 */
  //  this.createdAlert();
  },
  data() { /* 변수를 선언하는 곳 */
    return {
      count: 0,
      searchPh: '',
    }
  },
  methods: {
    createdAlert() {
      alert("ok");
    },
    plus() {
      this.count = this.count + 1;
    },
    minus() {
      this.count -= 1;
    }
  },
  props: {
    placeholderText: String
  }


}
</script>

<style scoped>

</style>