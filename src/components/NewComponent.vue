
<template>
    
</template>

<!--
<template>
    <h2> My FullName is {{ firstName }} {{ lastName }}</h2>
    <h2> computed {{ fullName }}</h2>

    <button @click="changeName">Change name </button>
    <h2 v-for="item in items" key="id">{{ item.fruit }} {{ item.snacks }}</h2>
    <h2>{{ total }}</h2>
    <button  @click="itemsPrice.push({id:4, item:'choco', price:400})">Add to Cart</button>

 
        <h2 v-for="items in expensiveItems" key="items.id">{{ items.item }} {{ items. price }}</h2>
   
</template>


<script>
export default{
    name: '',
    data(){
        return{
            firstName: 'Bruce',
            lastName: 'Lee',
            items:[
                {fruit: 'mango',},
                {snacks: 'oats'}


            ],

            itemsPrice:[
                {
                    id: 1,
                    item: 'Milk',
                    price: 600
                },
                {
                    id: 2,
                    item: 'Books',
                    price: 500
                },
                {
                    id:3,
                    item:'Fruits',
                    price:400
                }
            ]

        }
    },
    methods:{},
    computed: {

        changeName(){
            return this.fullName ='kent clark'

        },
        fullName: {
            get(){
                return `${this.firstName} ${this.lastName}`
            },
            Set(value){
                const name = value.split('')
                this.firstName = name[0]
                this.lastName= name[1]

            }
        

        },
       total(){
       return this.itemsPrice.reduce((total, curr) => (total= total + curr.price), 0)
       },

       expensiveItems(){
        return this.itemsPrice.filter(itemsPrice => itemsPrice.price > 400)
       }
    }
}

</script>

<style>

</style>
-->
