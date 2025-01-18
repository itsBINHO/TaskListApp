<template>
  <div class="category">
    <h2>Dance/Pop</h2>
  </div>
</template>

<script>
  export default {
    name: 'Category'
  }
</script>

<style>
  .category {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 80px;
    margin-left: 27vw;
  }
  @media (max-width: 768px) {
  .category {
    display: flex;
    align-items: center;
    margin-top: 80px;
    margin-right: 2em;
    margin-left: 2vw;
  }
}
@media (max-width: 480px) {
  .category {
    display: flex;
    height: 40px;
    align-items: center;
    margin-top: 10px;
    margin-right: 2em;
    margin-left: 1vw;
  }
}
</style>