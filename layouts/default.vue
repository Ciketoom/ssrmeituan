<template>
  <el-container class="layout-default">
    <el-header height="197px">
    	 <my-header/>
    </el-header>
    <el-main>
  	   <my-main/>
    </el-main>
    <el-footer height="100%">
      <my-footer/>
    </el-footer>
  </el-container>
</template>

<script>
import MyHeader from '@/components/public/header/index.vue'
import MyFooter from '@/components/public/footer/index.vue'
import MyMain from '@/pages/index.vue'
export default {
	 components:{
	 	 MyHeader,
	 	 MyMain,
	 	 MyFooter
	 }
}
</script>
