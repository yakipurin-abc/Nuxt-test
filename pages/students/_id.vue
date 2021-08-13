<template>
  <div class="student_id">
    <div>
      <p>{{ this.$route.params.user}}</p>
      <div class="link">
        <NuxtLink to='/students' class="student-link">生徒一覧へ戻る</NuxtLink>
        <p>|</p>
        <NuxtLink to='/' class="top-link">トップページへ</NuxtLink>
      </div>
    
    </div>
  </div>
</template>


<script>
export default {

  data() {
    return {
      students: [
        {
          id: "qnfungqxllc3m1ak",
          name: "生徒A",
        },
        {
          id: "7j9cumkgsq6l264c",
          name: "生徒B",
        },
        {
          id: "eo34bhey9m0d92ou",
          name: "生徒C",
        },
      ],
      user: '',
    }
  }
};
</script>


<style>
.student_id {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.link{
  display: flex;
  justify-content: center;
  align-items: center;
}
.link p{
  font-size: 14px;
  margin:0 15px;
}
.top-link{

}
</style>