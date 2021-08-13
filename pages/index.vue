<template>
  <div class="container">
    <div class="container-item">
      <div class="student">
        <p>生徒一覧</p>
        <NuxtLink to='/students' >生徒の情報を見る</NuxtLink>
      </div>
      <div class="administrator">
        <p>管理者</p>
        <NuxtLink to='/management' >管理画面を見る</NuxtLink>
      </div>
    </div>
  </div>
</template>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.container-item p{
  font-size: 20px;
  font-weight: bold;
}
.container-item{
  display: flex;
  justify-content: center;
  align-items: center;
}
.student{
  margin: 20px;
}
.administrator{
  margin: 20px;
}
</style>