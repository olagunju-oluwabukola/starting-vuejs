<template>
    <div class="div">
        <h1 class="text">{{ text }}</h1>
    <h2 class="text">{{ num }}</h2>
    <button @click="toggleModal()">showModal</button>

    </div>
   
   <div class="backdrop"v-if="showModal" @click="closeModal">

    <div class="modal"  >
       
            <h1 class="title" @click.left="closeModal()">{{ modal }}</h1>
            <h1></h1>
       
        

    </div>

   </div>
</template>

<script>
export default{
    props:['title', 'num', 'modal'],
 
    data(){
        return{
            text: 'Vuejs Tutorial',
            showModal:false
        }

      

    },
     methods:{
        toggleModal(){
            this.showModal=!this.showModal
        },
        closeModal(){
          this.showModal=!this.showModal
        }
     }
}
</script>

<style>
body{
    background: white;
    height: 100vh;
    color: black;
}

.modal{
    width: 400px;
    padding: 20px;
    margin: 100px auto;
    background: white;
    border-radius: 10px;

}

.backdrop{
   top: 0;
   position: fixed;
   background: rgba(0,0,0,0.5);
   width: 100%;
   height: 100%;
   
}


.div{
    display: block;
    text-align: center;
}
</style>