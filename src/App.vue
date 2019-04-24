<template>
    <div id="app">
       <Header :title='title' />
       <img src="./assets/logo.png">
       <h1>{{ hello }}</h1>
       <ul>
           <li v-for="(item, index) in list">
               {{ index + 1 }} {{ item }}
           </li>
           <li v-for="person in people">
               {{ person.name }}
           </li>
           <li v-for="(value, key) in profile">
               {{ key }}: {{ value  }}
           </li>
           </ul>
       <!-- <HelloWorld 
       :key="person.id"
       v-for="person in people"
       msg="Welcome"/> -->
       <HelloWorld msg="Welcome"/>
    </div>
</template>


<script>
import HelloWorld from './components/HelloWorld.vue';
import Header from './components/Header.vue';

export default {
    name: 'app',
    data(){
        return {
            hello: 'HEllo World',
            title: 'Test movie Fonts',
            list: [
                "Horse",
                "Penguin",
                "Lion",
                "Giraffe",
                "Dragon",
                "OC DAWGS"
            ],
            people: [
                {
                    id: "as1222",
                    name: "Ernie"
                },
                {
                    id: "as1244534",
                    name: "Eliamer"
                },
                {
                    id: "aopwjehehe",
                    name: "Bbong"
                },
                {
                    id: "00oapsjd",
                    name: "Bebe"
                }
            ],
            profile: {
                name: "Ernie",
                age: 18,
                job: "Senior Developer"
            }
        };
    },
    components: {
        HelloWorld,
        Header
    }
};
</script>

<style>
    body {
        margin: 0;
    }
  
    li{
        text-decoration-style: none;
        list-style-type: none;
    }

#app {
   font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
   }
</style>


