<!--
  Created by KanadeM on 2020/10/4
-->
<template>
  <div>
    <editor
        api-key="no-api-key"
        :init="{
         height: 500,
         menubar: false,
         plugins: [
           'advlist autolink lists link image charmap print preview anchor',
           'searchreplace visualblocks code fullscreen',
           'insertdatetime media table paste code help wordcount'
         ],
         toolbar:
           'undo redo | formatselect | bold italic backcolor | \
           alignleft aligncenter alignright alignjustify | \
           bullist numlist outdent indent | removeformat | help'
       }"
    />
  </div>
</template>

<script>
  import Editor from '@tinymce/tinymce-vue'
  export default {
    name: "rishtext-article",
    components: {
      'editor': Editor
    }
  }
</script>

<style scoped>

</style>
