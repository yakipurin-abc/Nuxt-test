<template>
  <div class="management">
    <div>
      <p class="asdf">生徒管理ページ</p>
      <table cellpadding="20px">
        <tr>
          <th>名前</th>
          <th>ID</th>
        </tr>
        <tr v-for="student in students" :key="student.id">
          <td class="student-name">{{student.name}}</td>
          <td class="student-ID">{{student.id}}</td>
        </tr>
      </table>
      <NuxtLink to='/'>戻る</NuxtLink>
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
    };
  },
};
</script>


<style>
.management {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
p{
  font-size: 30px;
  font-weight: bold;
  margin-bottom: 0;
}

</style>