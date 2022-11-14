<template>
<div class="main-container">
    <div class="project-card" v-for="(items, index) in projectData.projectsArray" v-bind:key="items">
        <h2>{{projectData.projectsArray[index].Title}}</h2>
        <img class="card-image" :src="projectData.projectsArray[index].Image" alt="">
        <div class="links">
            <a :href="projectData.projectsArray[index].Link1" target="_blank"><img src="../assets/paperclip-solid.svg" alt=""></a>
            <a :href="projectData.projectsArray[index].Link2" target="_blank"><img src="../assets/github1.svg" alt=""></a>
        </div>
    </div>
</div>
</template>

<script>
import jsonData from "/projects.json"
export default {
    data(){
        return{
            projectData: jsonData
        }
    }
}
</script>

<style scoped>

.main-container{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
}

.project-card{
    margin: 10px;
    padding: 10px;
    flex-wrap: 0 0 40%;
    /* outline: 1px solid black; */
    border-radius: 6px;
    box-shadow: rgb(144, 144, 144) 0px 3px 8px;
}

.project-card img{
    height: 9rem;
    border-radius: 4px;
    /* outline: 1px solid black; */
}

.card-image{
        outline: 1px solid black;
}

.links img{
    height: 25px;
    margin: 5px 10px 0 10px;
    transition-duration: .3s;
    opacity: 80%;
    border-radius: 40%;
}

.links img:hover{
    cursor:pointer;
    opacity: 60%;
}
</style>