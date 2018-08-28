<template>
    <div>
        <h1>Money</h1>
        <input type="text" v-on:keyup="pressKey" v-model="current" placeholder="Income">
        <!-- <p>Your tax bracket is: {{ income || 0 }}</p> -->
        <p>Your tax bracket is: {{ current || 0 }}</p>
        <button @click='clear'></button>
        <button @click='add'></button>
        <button v-on:click='add'></button>
        <div>

        </div>
    </div>
</template>

<script>
    export default {
        name: 'Money',
        data() {
            return {
                current: 'fff'
            }
        },
        props: {
            msg: String
        },
        methods: {
            add() {
                this.current = this.current + 1;
            },
            clear() {
                this.current = '';
            },
            pressKey: function(e) {
                console.log(e.target.value);
            }
        },
        
    }
</script>

<style lang="scss" scoped>
    h1 {
        font-size: 3em;
        color: red;
    }
</style>

    
  