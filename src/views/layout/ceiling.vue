<template>
  <div class="layout-ceiling">
    <!--<Avatar class="align-middle avatar" shape="square" src="https://i.loli.net/2017/08/21/599a521472424.jpg" />-->

    <Dropdown style="float: right" placement="bottom-end">
        <!--<Avatar class="avatar"  shape="square" src="https://i.loli.net/2017/08/21/599a521472424.jpg" />-->
      <Button type="text" style="margin-top: -3px; margin-right:-10px;">
        <Avatar class="avatar"  shape="square" src="https://i.loli.net/2017/08/21/599a521472424.jpg" />
      </Button>
      <DropdownMenu slot="list">
        <DropdownItem>个人设置</DropdownItem>
        <DropdownItem divided>退出登录</DropdownItem>
      </DropdownMenu>

    </Dropdown>
    <div class="layout-ceiling-main align-middle" >
      <a href="#/login">注册登录</a>
      <a href="#">帮助中心</a>
      <a href="#">安全中心</a>
      <a href="#">服务大厅</a>

    </div>



  </div>
</template>
<style scoped>
  .layout-ceiling {
    background: #464c5b;
    /*padding: 10px 0;*/
    height: 40px;
    overflow: hidden;
  }

  .layout-ceiling-main {
    float: right;
  }

  .layout-ceiling-main a {
    border-left: 1px solid #cccccc;
    color: #9ba7b5;
    padding: 0 10px;
    margin: 10px 0;
    text-align: center;
    cursor: pointer;
    font-size: 14px;
    line-height: 14px;
    position: relative;
  }

  .layout-ceiling-main a:hover {
    color: #fff;
  }
  .layout-ceiling .avatar {
    float: right;
    margin-right: 1em
  }
</style>
<script>
  export default {
    name: 'ceiling',
    props: {
      itemList: Array
    }
  }
</script>
