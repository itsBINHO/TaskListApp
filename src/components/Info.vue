<template>
  <div class="info">
    <h2 >{{ nome }}</h2>
      <h4 class="ml-7">With "Bad Guy", she became the first <br> 
        artist born in the 21st century and third <br>
        Gen Z artist <a href="#">MORE</a></h4>
      </div>
</template>

<script>
  export default {
    name: 'Info',
      data: () => {
        return {
          nome: 'Billie Eilish',
      }
    }
  }
</script>

<style>

  .info {
    margin-left: 2em;
  }
  .info h2 {
    font-size: 40px;
    font-weight: bold;
    margin-top: 50px;
    margin-left: 27px;
    margin-bottom: 10px;
  }

  a {
    text-decoration: none;
    color: #6687FF;
  }

  .info h4 {
    color: rgb(152, 158, 163);
  }
  @media (max-width: 480px) {
  .info{
    display: flex;
    flex-direction: column;
    margin-top: 1em;
    margin-left: 0;
    width: 22%;

  }
  .info h2 {
    display: flex;
    font-size: 22px;
    margin-top: 2em;
  }
  .info h4 {
    display: none;
  }
}
</style>