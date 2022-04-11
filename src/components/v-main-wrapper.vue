<template>
    <div class="v-main-wrapper">
        <v-catalog></v-catalog>
        <v-vart/>

    </div>
</template>

<script>
    import vCatalog from './v-catalog.vue';
    import VVart from './v-vart.vue';
    export default {
        name: 'v-main-wrapper',
        components: {//Дочерние элементы
            vCatalog,
                VVart,
        },
        props:{},
        data(){//То что можем передать и содержится в компоненте
            return{
                title: 'Main wrapper'
            }
        },
        computed: {
        },
        methods: {},//Клики, модальные окна и вся фигня от пользователя
        watch: {}, //Отлавливать изменения 
        mounted(){//Хук срабатывает при полной загрузке компонента
            console.log('Hello!')
        }
    }
</script>

<style style="scss">
    .v-main-wrapper{
        max-width: 900px;
        margin: 0 auto
    }
</style>