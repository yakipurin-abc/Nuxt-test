<template>
  <div class="students">
    <div>
      <p>生徒一覧</p>
      <ul v-for="student in students" :key="student.name">
        <li>
          <NuxtLink :to="{name: 'students-id', params: {user: student.name}}">{{student.name}}</NuxtLink>
        </li>
      </ul>
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
.students {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
p{
  font-weight: bold;
  font-size: 30px;
}
</style>