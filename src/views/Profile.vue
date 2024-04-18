<template>
  <div>
    <div>
      <img
        src="https://pbs.twimg.com/profile_images/1734389719759196160/yL-AeF_d_400x400.jpg"
        alt="img-perfil"
      />
      <h2>{{ $auth.user.name }}</h2>
      <p>{{ $auth.user.email }}</p>
    </div>

    <div>
      <pre>{{ JSON.stringify($auth.user, null, 2) }}</pre>
    </div>
  </div>
</template>
<style scoped>
img {
  border-radius: 50%;
  width: 100px;
  height: 100px;
}
pre {
  background-color: #f4f4f4;
  padding: 20px;
  border-radius: 5px;
  overflow: auto;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  line-height: 2;
}
</style>