<template>
    <section class="mixins_container">
        <a href="#" class="my_button">Bottone</a>
        <a href="#" class="my_button2">Bottone 2</a>
    </section>
    
</template>

<script>
export default {
    name: 'SassTitle',
    data: function(){
        return {

        };
    }
}
</script>

<style lang="scss" scoped>
    @mixin base_button{
        padding: 10px;
        color: red;
        text-decoration: underline;
        background-color: purple;
    }
    .my_button{
        @include base_button;
    }
    .my_button2{
        @include base_button;
        text-transform: uppercase;
    }

    
</style>