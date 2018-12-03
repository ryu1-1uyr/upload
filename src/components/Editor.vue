<template>
<div id="app">
  <div class="editor">
    <mavon-editor ></mavon-editor>
  </div>
  <button @click="getMsg">getMsg</button>
  <div>{{ message }}</div>
</div>
  </template>

<script>
  import Vue from 'vue'
  import mavonEditor from 'mavon-editor'
  import 'mavon-editor/dist/css/index.css'

  Vue.use(mavonEditor)
  new Vue({
    el: '#app',
    data() {
      return {
        //mavon-editor
        toolbars: {
          bold: false,
        },
        //other
        message: ''
      }
    },
    methods: {
      $imgAdd(pos, $file) {
        alert('upload image');
      },
      $change(value, reader) {
        this.message = value
      },
      getMsg() {
        console.log(this.message)
      }
    },
  })

  // export default {
  //   name: 'suggest',
  //   data () {
  //     return {
  //     }
  //   },
  //   methods : {
  //
  //   },
  //   comments : {
  //     mavonEditor
  //   }
  // }


  /*
  *
  *   export default {
    name: 'suggest',
    data () {
      return {
        emojiList: emojiOrigin,
        preConvertEmoji: ""
      }
    },
    methods: {

      enter: function(data){

        this.$emit('enter', data.target.value)

      }
    }
  }
  *
  * */

</script>
