<template>
    <div class="theEngine" v-if="engines.length">
        <div v-for="items in engines" key="items" class="card">
            <img :src="items.image" alt="">
        <div class="container">
            <p>{{items.engineName}}</p>
            <p>{{items.price}}</p>
            <button>Buy Engine</button>
        </div>
        </div>
    </div>
    <div v-else>
        <p>Products loading ..</p>
        <Spinner />
    </div>
</template>

<script>
import Spinner from '@/components/Spinner.vue'
    export default {
        components: {
            Spinner
        },
        name: 'Products',
        data(){
            return {
                engines :[
                {
                    id: 1,
                    image:'https://i.postimg.cc/P502Rvv2/1965-ford-mustang-with-rb26-nissan-gt-r-engine-is-a-tokyo-drift-tribute-5.jpg',
                    engineName: 'RB26',
                    price:'R 55 000.00'
                },
                {
                    id:2,
                    image:'https://i.postimg.cc/HxY5ZTz6/Screenshot-20210723-112523-Gallery.jpg',
                    engineName:'2JZ',
                    price:'R55 000.00'
                },
                {
                    id:3,
                    image:'https://i.postimg.cc/d3zhYFRP/38427-1663687277.jpg',
                    engineName: 'SR20',
                    price:'R20 000.00'
                },
                {
                    id: 4,
                    image:'https://i.postimg.cc/1XYjRC4Z/Screenshot_20210807-050555_Instagramb-951x1024.jpg',
                    engineName:'1JZ',
                    price:'R50 000.00'
                }
            ]
            }
        }   
    }
</script>

<style scoped>
.theEngine {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}
.card {
    width: 20%;  
}
.container {
    padding: 2px 16px;
}

img {
    width: 15rem;
    margin: auto;
    margin-top: 2rem;
}
</style>