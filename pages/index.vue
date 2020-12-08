<template>
 <div class="bg-gray-300 flex items-center justify-center py-32 px-4">
   <div class="max-w-sm w-full sapce-y-8">
     <div>
       <img  class="m-auto w-10 h-10" src="https://tailwindui.com/img/logos/workflow-mark-indigo-600.svg" alt="">
      <h2 class="text-center font-bold text-2xl" >Sign in to your account</h2>
      <div class="flex flex-row justify-center text-sm space-x-1">
        <span>Or</span>
        <a href="#" class="text-blue-700">start your 14-day free trial</a>
      </div>
     </div>
     <div class="flex flex-col border-solid rounded-sm bg-white h-96 w-96 my-8 py-6 px-6 border-gray-300">
       <div class="flex flex-col my-4">
        <span class="text-sm">Email Address</span>
        <el-input v-model="input"></el-input>
       </div>
         <div class="flex flex-col">
        <span class="text-sm">Password</span>
        <el-input v-model="input2" show-password></el-input>
       </div>
       <div class="flex flex-row justify-between my-4">
           <el-checkbox v-model="checked">Remember me</el-checkbox>
           <a href="#" class="text-purple-700">Forgot your password?</a>
       </div>
      
      <div class="bg-purple-700 border-gray-300 rounded-sm text-white text-center">
          <el-button>Sign In</el-button>
      </div>

      <div class="flex flex-row items-center justify-center">
        <div class="divide-y divide-gray-300">
        <div>&nbsp;</div>
        <div>&nbsp;</div>
        </div>
        <span class="text-center text-gray-700">Or continue with</span>
        <div class="divide-y divide-gray-300">
        <div>&nbsp;</div>
        <div>&nbsp;</div>
        </div>
      </div>

      <div class="flex flex-row space-x-4 justify-center">
        <el-button ></el-button>
        <el-button icon="el-icon-share"></el-button>
        <el-button icon="el-icon-delete"></el-button>
      </div>
     </div>
     
   </div>
 </div>
 </template>

 
<script>
export default {
  data() {
    return {
      input: '',
       checked: true,
       input2: '',
    }
  }
}
</script>