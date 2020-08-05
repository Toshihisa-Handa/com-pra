<template>
  <v-container>
    <v-row justify="center" align="center">
      <v-col cols="12">

      <LoginForm/>
      <ButtonForm/>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import LoginForm from '../components/LoginForm'
import ButtonForm from '../components/ButtonForm'

export default{
    name:'Login',//ここの名前は任意設定
    
    components:{
        LoginForm,//ここの記載をtemplateで呼び出す際に使う
        ButtonForm,
    },
}



</script>