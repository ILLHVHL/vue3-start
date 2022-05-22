<template>
  <table id="board">
    <thead>
      <tr>
        <th> No. </th>
        <th> 제목 </th>
      </tr>
    </thead>
    <tbody>
    <tr v-for="(data, index) of boardArray" :key="index">
      {{ index }}
      <td>
      {{ data.seq }}
      </td>
      <td>
        {{ data.title }}
      </td>
    </tr>
    </tbody>
  </table>
</template>

<script>
export default { /* BoardComponent 라는 이름으로 화면을 내보내기 위함 */
  name: "BoardComponent",

  data() {
    return {
      boardArray: [
        { seq: 1, title: 'test1' },
        { seq: 2, title: 'test2' },
        { seq: 3, title: 'test2' }
      ]
    }
  }
}
</script>

<style scoped>

</style>