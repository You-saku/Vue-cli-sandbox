<template>
    <h1>Shopping</h1>
    <h2>Counter</h2>
    <p>Count : {{ counter }}</p>
    <span v-if="seen">You can see!!</span>
    <button v-on:click="counter+=1">Add</button>
    <button v-on:click="sub">Sub</button>
    <button v-on:click="counter=0">Reset</button>

    <h2>Item</h2>
    <p>Price : {{price}} ¥</p>

    <h2>Total Amount</h2>
    <p>Total Amount : {{totalPrice}} ¥</p>

    <h1>I lived those prefectures.</h1>
    <ul>
    <li v-for="prefecture in prefectures" :key="prefecture.item">
        {{ prefecture.item }}
    </li>
    </ul>

</template>

<script>
export default {
    name: 'Sample1',
    data(){
        return{
            counter: 0,
            price: 100,
            seen: false,
            prefectures: [
                {item: 'Gunmma'},
                {item: 'Saitama'},
                {item: 'Tokyo'},
            ],
        }
    },

    methods: {
        sub: function(){
            this.counter--;
            if(this.counter < 0){
                this.counter = 0;
            }
        }
    },
    
    computed: {
        totalPrice: function(){
            if(this.counter < 0){
                return 0;
            }else{
                return this.counter * this.price;
            }
        }
    }
}
</script>

<style scoped>
    ul {
        list-style-type:none;
        display: inline;
    }
</style>