<template>

    <div id="all">
        <Mytitle/>
        <Markdown
            v-model="val"
            @on-ready="onReady"
            @on-copy="onCopy"
            @on-upload-image="onUpladImage"
            @on-save="onSave"
            :height="500"
        />
    </div>
</template>

<script>

    import Markdown from './components/pro/index';
    import Mytitle from './components/title/mytitle'

    export default {
        components: {
            Mytitle,
            Markdown
        },
        data: function () {
            return {
                val: ''
            }
        },
        methods: {
            onReady(data) {
                console.log(data)
            },
            onCopy(text) {
                console.log(text);
            },
            onUpladImage(file) {
                console.log(file)
            },
            onSave(data) {
                console.log(data);
            }
        }
    }
</script>

<style lang="less">
  #all
  {
      position:absolute;
      width: 100%;
      height: 100%;
      overflow: auto;
  }
</style>