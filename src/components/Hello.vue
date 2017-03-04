<template>
  <div>
    <span class="title">欢迎登录</span>
    <divider>Vue Vux</divider>
    <Group>
      <XInput title="账号" v-module='account' placeholder='账号' type='text'></XInput> 
      
    </Group>
    <XInput title="密码" v-module='password' placeholder='密码' type="password"></XInput>
    <XButton type="primary" action-type="button">登录</XButton>
  </div>
</template>

<script>
  import { Divider, Group, XInput, XButton } from 'vux'
  export default {
    components: {
      Divider,
      Group,
      XInput,
      XButton
    },
    data () {
      return {
        account: '',
        password: ''
      }
    }
  }
</script>
