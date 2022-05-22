<template><!-- html 같은 역할 -->
  <div class="about">
    <h1>This is an about page</h1>

    <search-component
        :placeholderText = "'ㅛㄱ용요요'" />
    <board-component /> <!-- script에서 components에서 사용하겠다고 지시해서 태그로 만들어진 거임 명칭은 케밥케이스로 호출하는 것이 원칙 -->

  </div>
</template>

<script> /* 코드 작성 */
import BoardComponent from "@/components/BoardComponent";
import SearchComponent from "@/components/SearchComponent";

export default {
  name : 'about-view',
  components : { /* import 시킨 컴포넌트 파일들을 사용하겠다고 지시 */
    BoardComponent,
    SearchComponent
  },
  data() {
    return {
      test: '바보'
    }
  }

}
</script>

<style lang="scss">/* css */
</style>
