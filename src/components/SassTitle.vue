<template>
    <section class="subtitles_container">
        <h3 class="title">Titolo Principale</h3>
        <h4 class="subtitle">Sottotitolo</h4>
        <h5 class="subsubtitle">Altro sottotitolo <h5 class="subsubtitle_sub">prova</h5></h5>
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
    $title_primary_color: red;
    $title_secondary_color: greenyellow;
    .subtitles_container{
        color: blue;
        .title{
            color: $title_primary_color;
            background-color: $title_secondary_color;
        }
        .subtitle{
            color: $title_secondary_color;
            background-color: $title_primary_color;
        }
        & > h5{
            font-family: cursive;
            cursor: pointer;
            text-decoration: underline;
            .subsubtitle_sub{
                display: inline-block;
                color: purple;
            }
            &:hover{
                transform: scale(2);
            }
        }
    }
    
</style>