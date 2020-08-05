<template>
  <v-container>
    <v-row justify="center" align="center">
      <v-col cols="12">

      <FormList/>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import FormList from '../components/FormList'

export default{
    name:'Form',//ここの名前は任意設定
    
    components:{
        FormList,//ここの記載をtemplateで呼び出す際に使う
    },
}



</script>