<template>
  <div class='hi'>
    Hi Vue!
    <h1>
      {{message}}
    </h1>
    <button @click="show_my_value()">显示初始值</button>
  </div>
</template>

<script>
export default {
  data () {
    return {
      message: '你好Vue，我是message的初始值'
    }
  },
  methods: {
    show_my_value: function () {
      alert('my_value: ' + this.message)
    }
  }
}
</script>

<style>
.hi {
  color: red;
  font-size: 20px;
}
</style>
