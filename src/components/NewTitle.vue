<template>
    <section class="title_container">
        <input :maxlength="titleLength" v-model="userTitle" @keyup.enter="getUserTitle" class="user_input" type="text" placeholder="Inserisci il titolo qui">
        <h2 v-if="titleShowed">{{userTitle}}</h2>
    </section>
</template>

<script>
export default {
    name: 'NewTitle',
    data: function(){
        return {
            userTitle: '',
            titleShowed: false,
            titleLength: null
        };
    },
    methods: {
        getUserTitle: function(){
            this.titleShowed = true
            this.titleLength = this.userTitle.length;
        }
    }
}
</script>

<style scoped>
    .title_container{
    background-color: black;
    width: 100%;
    height: 50vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    }
    .user_input{
        padding: 5px;
        color: aqua;
    }
    h2{
        color: aqua;
    }
    
</style>