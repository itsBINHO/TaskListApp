<template>
  <div class="category">
    <h2>Dance/Pop</h2>
    <div class="buttons-track d-flex mt-2 ">
      <v-btn variant="plain">
        <a href="#">
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M29.3113 13.8838L11.3013 2.8675C10.9236 2.63725 10.4915 2.51133 10.0493 2.5026C9.60702 2.49387 9.17036 2.60264 8.78387 2.81781C8.39739 3.03297 8.07491 3.34683 7.84936 3.72735C7.6238 4.10787 7.50325 4.54142 7.5 4.98375V27.0163C7.50325 27.4586 7.6238 27.8921 7.84936 28.2727C8.07491 28.6532 8.39739 28.967 8.78387 29.1822C9.17036 29.3974 9.60702 29.5061 10.0493 29.4974C10.4915 29.4887 10.9236 29.3628 11.3013 29.1325L29.3113 18.1163C29.6744 17.8952 29.9746 17.5844 30.1828 17.2138C30.3911 16.8431 30.5005 16.4251 30.5005 16C30.5005 15.5749 30.3911 15.1569 30.1828 14.7862C29.9746 14.4156 29.6744 14.1048 29.3113 13.8838ZM10.5 26.1063V5.89375L27.02 16L10.5 26.1063Z" fill="#F8F8F8"/>
          </svg>
        </a>
      </v-btn>
      <v-btn variant="plain">
        <a href="#">
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M32 18.2857H18.2857V32H13.7143V18.2857H0V13.7143H13.7143V0H18.2857V13.7143H32V18.2857Z" fill="#F8F8F8"/>
          </svg>
        </a>
      </v-btn>
      <v-btn variant="plain">
        <a href="#">
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M8 28V25.3333C8 23.9188 8.5619 22.5623 9.5621 21.5621C10.5623 20.5619 11.9188 20 13.3333 20H18.6667C20.0812 20 21.4377 20.5619 22.4379 21.5621C23.4381 22.5623 24 23.9188 24 25.3333V28M10.6667 9.33333C10.6667 10.7478 11.2286 12.1044 12.2288 13.1046C13.229 14.1048 14.5855 14.6667 16 14.6667C17.4145 14.6667 18.771 14.1048 19.7712 13.1046C20.7714 12.1044 21.3333 10.7478 21.3333 9.33333C21.3333 7.91885 20.7714 6.56229 19.7712 5.5621C18.771 4.5619 17.4145 4 16 4C14.5855 4 13.229 4.5619 12.2288 5.5621C11.2286 6.56229 10.6667 7.91885 10.6667 9.33333Z" stroke="#F8F8F8" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </a>
      </v-btn>
      <v-btn variant="plain">
        <a href="#">
          <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path fill-rule="evenodd" clip-rule="evenodd" d="M32 4.26666H0V2.13333H32V4.26666ZM32 12.8H0V10.6667H32V12.8ZM32 21.3333H0V19.2H32V21.3333ZM32 29.8667H0V27.7333H32V29.8667Z" fill="#F8F8F8"/>
          </svg>
        </a>
      </v-btn>
    </div>
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
</style>