<template>
  <div id="panel-container">
    <h3><strong>{{labelID}}</strong></h3>
  </div>
</template>

<script>
export default {
    name: "Panel",
    props: {
        labelID : Number,
        categoryID : Number,
        name : String,
        panelName : String,
    },
    data() {
        return {
        }
    },
}
</script>

<style scoped>
    #panel-container {
        border: solid black 1px;
        height: 250px;
        width: 250px;
    }
</style>