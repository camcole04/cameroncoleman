<script>
    import linkedinlogo from '$lib/assets/linkedin.svg';
    import githublogo from '$lib/assets/githublogo.png';
    import brushstroke from '$lib/assets/brushstroke.png';
</script>

<div >
    
    
    <div class="centered title-box">
        <div class="centered menu-title">
            <p>CAMERON COLEMAN</p>
            <p class="subtitle">4th Year Software Engineer | Rochester Institute of Technology</p>
            <a href="https://www.linkedin.com/in/cameron-coleman-swen">
                <img 
                    src={linkedinlogo}
                    style="width:42px;height:42px;"
                    alt="Cameron's LinkedIn">
            </a>
            <a href="https://github.com/camcole04">
                <img 
                    src={githublogo}
                    style="width:42px;height:42px;"
                    alt="Cameron's GitHub">
            </a>
        </div>
            <div class="background-image" style="background-image: url({ brushstroke });">
                <p class="projects">PROJECTS </p>
            </div>
            <p class="project"><a href="/projects/midiaudioplayer" >Midi Audio Player</a> </p>
    </div>
</div>



<style>
    @import url('https://fonts.googleapis.com/css2?family=Alegreya+Sans&display=swap');

    .background-wrapper {
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 50px;
    }

    .background-image {
        /* position: absolute; */
        padding: 10px; 
        background-size: cover;
        height: 100px;
        /* background-position: 50%; */
    }

    .centered {
        margin: 0 auto;
    }

    .title-box {
        padding: 100px 250px 50px 250px;
        height: 1300px;
        margin-top: 50px;
        width: fit-content;
        background-color: #70D6FF;
        font-family: 'Alegreya Sans', sans-serif;
        z-index: 1;
        position: relative;
    }

    .menu-title {
        background-color: #FF70A6;
        border: 6px solid #E9FF70;
        margin-top: -50px;
        padding: 50px;
        padding-top: 0px;
        font-size: 60px;
        width: fit-content;
    }

    .subtitle {
        margin-top: -70px;
        text-align-last: center;
        font-size: 18px;
        font-family: cursive;
    }

    .projects {
        margin: auto;
        font-family: 'Alegreya Sans', sans-serif;
        padding-top: 50px;
        font-size: 60px;
        color: white;
        width: fit-content;
    }

    .project {
        margin: auto;
        font-family: 'Alegreya Sans', sans-serif;
        font-size: 24px;
        color: white;
        width: fit-content;
    }

    a {
        text-decoration:none;
    }

    a:visited {
        color: white;
    }

    a:active {
        color: white;
    }

    a:hover {
        color: white;
    }
</style>