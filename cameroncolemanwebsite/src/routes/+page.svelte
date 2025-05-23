<script>
    import linkedinlogo from '$lib/assets/linkedin.svg';
    import githublogo from '$lib/assets/githublogo.png';
    import brushstroke from '$lib/assets/brushstroke.png';
    import emailicon from '$lib/assets/emailicon.png';
</script>

<div >
    
    
    <div class="centered page-box">
        <div class="centered menu-title">
            <p>CAMERON COLEMAN</p>
            <p class="subtitle">4th Year Software Engineer | Rochester Institute of Technology</p>
            <div class="links">
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
            <a href="mailto:nycolemans04@outlook.com">
                <img 
                    src={emailicon}
                    style="width:42px;height:42px;"
                    alt="Send me an email!">
            </a>
            </div>
        </div>
            <div class="section-title-background" style="background-image: url({ brushstroke });" >
                <p class="section-title"><a href="/aboutme">ABOUT ME </a> </p>
            </div>
            <div class="section-title-background" style="background-image: url({ brushstroke });">
                <p class="section-title">PROJECTS </p>
            </div>
            <p class="project"><a href="/projects/midiaudioplayer">Midi Audio Player</a> </p>
    </div>
</div>



<style>
    @import url('https://fonts.googleapis.com/css2?family=Alegreya+Sans&display=swap');
    @import '$lib/styles.css';

    .centered {
        margin-left: auto;
        margin-right: auto;
    }

    .menu-title {
        background-color: #FF70A6;
        border-radius: 20px;
        border: 6px solid #E9FF70;
        margin-top: -10px;
        margin-bottom: 50px;
        padding: 40px;
        padding-top: 0px;
        font-size: 60px;
        width: fit-content;
        max-height: 200px;
        box-shadow: 0 0 20px 20px #E9FF70;
    }

    .subtitle {
        margin-top: -70px;
        text-align-last: center;
        font-size: 18px;
        font-family: cursive;
    }

    .section-title {
        margin: auto;
        font-family: 'Alegreya Sans', sans-serif;
        font-size: 60px;
        width: fit-content;
    }

    .section-title-background {
        position: relative;
        display: flex;
        justify-content: center;
        margin-bottom: 50px;
        align-items: center;
        padding-top: 10px; 
        background-size: 350px 90px;
        background-repeat: no-repeat;
        background-position: 50%;
    }

    .project {
        margin: auto;
        font-family: 'Alegreya Sans', sans-serif;
        font-size: 24px;
        margin-top: -40px;
        width: fit-content;
    }

    .links{
        margin-left: 40%;
    }

    

</style>