<template>
  <main>
    <div class="container">
      <h2>--> Content goes here</h2>
    </div>
  </main>
</template>

<script>
export default {
  name: "Main",
}
</script>

<style lang="scss">

  main{
    background-color: #1c1c1c;

    .container{
      height: 150px;
      display: flex;
      align-items: center;
      color: white;
      h2{
        font-weight: 600;
      }
    }
  }
  
</style>