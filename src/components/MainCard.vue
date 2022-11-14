<template>
<div class="wrapper">
    <div class="main-container">
        <div class="container-one">
            <div class="profile">
                <img src="../assets/linkdinpic.png" alt=""/>
                <h6>Front-End Developer<br> Styling and Design Specialist <br> Fullstack Engineer</h6>
                <h6></h6>
                <h3>Contact Me!</h3>
            </div>
            <div class="social-links">
                    <div class="link">
                        <a href="https://github.com/MrTowelGuy" target="_blank">
                        <img src="../assets/square-github.svg" alt=""/>
                        </a>
                    </div>
                    <div class="link">
                        <a href="https://www.linkedin.com/in/jaden-garrity-96b33185/" target="_blank">
                        <img src="../assets/linkedin.svg" alt=""/>
                        </a>
                    </div>
        </div>
    </div>
        <div class="container-two">
            <div class="about-me">
                <h1>About Me</h1>
                <p>A creative mind based out of Atlanta, Ga. Huge lover of artistic media creation and design. Eager to learn new things, and pursue new amazing opportunities! Find me on Linkdin and Github, or checkout my projects below!</p>
            </div>
            <div class="technologies">
                <h1>Technologies Studied</h1>
                <p>More In Github Projects Details</p>
                <div class="logos">
                    <img src="../assets/html5.svg" alt="">
                    <img src="../assets/css3-alt.svg" alt="">
                    <img src="../assets/square-js.svg" alt="">
                    <img src="../assets/react.svg" alt="">
                    <img src="../assets/vuejs.svg" alt="">
                </div>
            </div>
            <div class="button-container">
                <div class="projects-button">
                    <a href="#">Projects</a>
                </div>
                <div class="projects-button">
                    <a href="#">Resume</a>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {

}
</script>


<style scoped>
.wrapper{
    display: flex;
    justify-content: center;

}

img{
    height: 40px;
}

.main-container{
    display:flex;
    flex-direction: row;
    background-color: rgb(255, 255, 255);
    /* outline: 1px solid black; */
    border-radius: 4px;
    box-shadow: rgb(177, 177, 177) 0px 6px 8px;
    width: 80%;
}

.container-one{
    background-color: rgb(255, 255, 255);
    outline: 1px solid black;
    padding: 2.5%;
    width: 30%;
    border-radius: 4px;
    margin: 2.5%;
}

.profile img{
    height: 5rem;
    border-radius: 50%;
    outline: 1px solid black;
}

.link a{
    text-decoration: none;
    color: black;
    font-size: 12px;
}

.link img:hover{
    color: rgb(135, 135, 135);
    opacity: 60%;
}

.link img{
    height: 3rem;
    transition-duration: .3s;
}


.container-two{
    background-color: rgb(255, 255, 255);
    outline: 1px solid black;
    border-radius: 4px;
    width: 70%;
    margin: 2.5%;
}

.about-me{
    text-align: left;
    padding-left: 15px;
    padding-right: 15px;
}

.logos img{
    height: 2.5rem;
    margin: 8px;
}

.button-container{
    margin-top: 3%;
    display:flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
}
.projects-button{
    background-color:rgb(29, 29, 29);
    border-radius: 15px;
    padding: 5px;
    margin: 5px;
}
.projects-button a{
    text-decoration: none;
    color: rgb(255, 255, 255);
    transition-duration: .3s;
}

.projects-button a:hover{
    opacity: 80%;
}

.technologies{
    text-align: left;
    padding-left: 15px;
    padding-right: 15px;
}

@media only screen and (max-width: 950px) {
    .main-container{
        width: 95%;        
    }
}

</style>