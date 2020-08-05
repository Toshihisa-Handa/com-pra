<template>
  <v-container>
    <v-row justify="center" align="center">
      <v-col cols="12">

      <ShopListForm/>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import ShopListForm from '../components/ShopListForm'

export default{
    name:'ShopList',//ここの名前は任意設定
    
    components:{
        ShopListForm,//ここの記載をtemplateで呼び出す際に使う
        
    },
}



</script>