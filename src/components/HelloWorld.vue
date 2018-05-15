<template>
  <v-container fluid>
    <v-layout column align-center class="mt-5">
      <div :id="this.$vuetify.breakpoint.name === 'xs' ||
                this.$vuetify.breakpoint.name === 'sm' ? '' : 'logo_wrap'">
        <img src="@/assets/icon/logo.svg" id="rehigh_logo" alt="Re:High Studio">
      </div>
      <p class="white--text">Хотите свой сайт? Свяжитесь с нами:</p>
      <v-chip color="accent">
        <v-avatar>
          <img src="@/assets/icon/contacts/vk.svg" height="30px" alt="">
        </v-avatar>
        <a href="https://vk.com/smelayapanda" target="_blank">Алексей Азаров</a>&nbsp&nbsp&nbsp
        <a href="https://vk.com/oliviacolin" target="_blank">Виктория Зайцева</a>
      </v-chip>
      <v-chip color="accent">
        <v-avatar>
          <img src="@/assets/icon/contacts/phone.svg" height="30px" alt="">
        </v-avatar>
        8 (999) 467 78 57 &nbsp/&nbsp 8 (923) 128 69 28
      </v-chip>
      <v-chip color="accent">
        <v-avatar>
          <img src="@/assets/icon/contacts/email.svg" height="30px" alt="">
        </v-avatar>
        ReHighStudio@gmail.com
      </v-chip>
      <v-chip color="accent">
        <v-avatar>
          <img src="@/assets/icon/contacts/inst.svg" height="30px" alt="">
        </v-avatar>
        <a href="https://www.instagram.com/rehighstudio/" target="_blank">Instagram</a>
      </v-chip>
    </v-layout>
  </v-container>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  a {
    color: #6a01be;
  }

  #rehigh_logo {
    height: 220px;
    margin-bottom: 20px;
  }
</style>
