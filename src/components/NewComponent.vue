<template>
    <h1>{{ title }} - {{ author }}</h1>
    <input type="text" ref="name">
    <button @click="handleClick" >Click Me</button>
    <button v-bind:open="isDisable">Bind</button>
    <h2 class="underline">Underline</h2>
<h2 v-bind:class="status">Status </h2>
<h2 v-bind:class="isPromoted && 'promoted'">Promoted movie</h2>
<h2 v-bind:class="isSoldOut ? 'soldout' : 'new'" >Sold out? movie</h2>
<h2 v-bind:style="dangerStyle">Danger style</h2>
<h2 v-bind:style="background">Success Style</h2>
<h2  class="gold" >Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur, modi?</h2>
<div>
    <h2 v-if="num===0">Number is Zero</h2>
    <h2 v-else-if="num > 0"> It is a positive number😘</h2>
    <h2 v-else-if="num < 0">It is a negative number😡</h2>
    <h2 v-else> Number is a negative</h2>
    
    
</div>
<h2 v-show="hideElement">Using v-show</h2>
</template>

<script>
export default {
    data(){
        return{
            num: 0,
            hideElement:true,
            name: 'app',
            title: 'My First Vue App',
            author : 'Me',
            isDisable: false,
            isPromoted: true,
            status: 'success',
            isSoldOut: true,
            style: 'gold',
             dangerStyle:{
                color: 'red',
                'font-size': '2em'
            
             },
             background: 'color:green',
             font :50,
            


        }
    },
    methods: {
        handleClick(){
            console.log('clicked')
        }
    }
}

</script>

<style scoped>

</style>
