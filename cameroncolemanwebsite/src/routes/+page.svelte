<script>
    import linkedinlogo from '$lib/assets/linkedin.svg';
    import githublogo from '$lib/assets/githublogo.png';
    import brushstroke from '$lib/assets/brushstroke.png';
    import emailicon from '$lib/assets/emailicon.png';

    import assemblyLogo from '$lib/assets/language_logos/assembly.png';
    import cLogo from '$lib/assets/language_logos/C.png';
    import cssLogo from '$lib/assets/language_logos/CSS.png';
    import htmlLogo from '$lib/assets/language_logos/HTML.png';
    import jsLogo from '$lib/assets/language_logos/javascript.png';
    import pgLogo from '$lib/assets/language_logos/postgresql.png';
    import pythonLogo from '$lib/assets/language_logos/python.png';
    import javaLogo from '$lib/assets/language_logos/java.png';
    import svelteLogo from '$lib/assets/language_logos/svelte.png';
    import kotlinLogo from '$lib/assets/language_logos/kotlin.png';

    import angularLogo from '$lib/assets/framework_logos/angular.png';
    import bootstrapLogo from '$lib/assets/framework_logos/bootstrap.png';
    import dockerLogo from '$lib/assets/framework_logos/docker.png';
    import flaskLogo from '$lib/assets/framework_logos/flask.svg';
    import gitLogo from '$lib/assets/framework_logos/git.png';
    import nodejsLogo from '$lib/assets/framework_logos/nodejs.png';
    import reactLogo from '$lib/assets/framework_logos/react.png';
    import springLogo from '$lib/assets/framework_logos/spring.png';
</script>

<div>
    <div class="centered page-box">
        <div class="centered menu-title">
            <p class="main-title">CAMERON COLEMAN</p>
            <p class="subtitle">4th Year Software Engineer | Rochester Institute of Technology</p>
            <div class="links">
                <a href="https://www.linkedin.com/in/cameron-coleman-swen">
                    <img 
                        src={linkedinlogo}
                        class="icon"
                        alt="Cameron's LinkedIn">
                </a>
                <a href="https://github.com/camcole04">
                    <img 
                        src={githublogo}
                        class="icon"
                        alt="Cameron's GitHub">
                </a>
                <a href="mailto:nycolemans04@outlook.com">
                    <img 
                        src={emailicon}
                        class="icon"
                        alt="Send me an email!">
                </a>
            </div>

        </div>
        
        <p class="section-title" style="margin-bottom: 120px; margin-top: 120px;"><a href="/aboutme">ABOUT ME </a> </p>
        
        <p class="section-title">PROJECTS </p>

        <hr class="section-divider" />
        
        <p class="project"><a href="/projects/midiaudioplayer">Midi Audio Microcontroller</a> </p>
        <p class="project"><a href="/projects/midiaudioplayer">Ultrasonic Musical Note Recognition Game</a> </p>
        <p class="project"><a href="/projects/midiaudioplayer">Hermes Navigation System (Front End)</a> </p>

        

        <!-- New Teck Stack Section -->
        <div class="teck-stack-section">
            <p class="section-title">Tech Stack</p>
            <hr class="section-divider" />
            <div class="subsection">
                <p class="subsection-title">Technical Languages</p>
                <div class="language-logos">
                    <img src={assemblyLogo} alt="Assembly" />
                    <img src={cLogo} alt="C" />
                    <img src={cssLogo} alt="CSS" />
                    <img src={htmlLogo} alt="HTML" />
                    <img src={jsLogo} alt="JavaScript" />
                    <img src={pgLogo} alt="PostgreSQL" />
                    <img src={pythonLogo} alt="Python" />
                    <img src={javaLogo} alt="Java" />
                    <img src={kotlinLogo} alt="Kotlin" />
                </div>
            </div>
            <div class="subsection">
                <p class="subsection-title">Frameworks</p>
                <div class="language-logos">
                    <img src={svelteLogo} alt="Svelte" />
                    <img src={angularLogo} alt="Angular" />
                    <img src={bootstrapLogo} alt="Bootstrap" />
                    <img src={dockerLogo} alt="Docker" />
                    <img src={flaskLogo} alt="Flask" />
                    <img src={gitLogo} alt="Git" />
                    <img src={nodejsLogo} alt="Node.js" />
                    <img src={reactLogo} alt="React" />
                    <img src={springLogo} alt="Spring" />
                </div>
            </div>
        </div>
    </div>

</div>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Great+Vibes&family=Palatino&display=swap');
    @import '$lib/styles.css';

    .centered {
        margin-left: auto;
        margin-right: auto;
    }

    .page-box {
        padding: 60px 40px 80px 40px;
        margin: 50px auto;
        width: 60%;
        background-color: #fdf6e3; /* warm cream */
        border: 2px solid #d2b48c; /* tan border */
        border-radius: 12px;
        box-shadow: 0 0 15px rgba(210, 180, 140, 0.5);
        font-family: 'Palatino', serif;
    }

    .main-title {
        font-family: 'Palatino', serif;
        font-size: 72px;
        color: #8b4513; /* saddle brown */
        margin-bottom: 0;
        text-align: center;
        letter-spacing: 2px;
    }

    .subtitle {
        font-family: 'Palatino', serif;
        font-size: 20px;
        color: #5a3e1b; /* dark brown */
        text-align: center;
        margin-top: 0;
        margin-bottom: 30px;
        font-style: italic;
    }

    .section-title {
        margin: auto;
        font-family: 'Palatino', serif;
        margin-top: 120px;
        margin-bottom: 120px;
        font-size: 76px;
        color: #8b4513;
        width: fit-content;
        text-align: center;
    }

    .section-title a {
        transition: transform 0.3s ease, filter 0.3s ease, text-shadow 0.3s ease;
        display: inline-block;
        text-decoration: none;
    }

    .section-title a:hover {
        transform: scale(1.1);
        filter: drop-shadow(2px 4px 6px rgba(0, 0, 0, 0.4));
        cursor: pointer;
        text-shadow: 1px 1px 2px rgba(0,0,0,0.6);
    }

    .project {
        margin: 20px auto;
        font-family: 'Palatino', serif;
        font-size: 36px;
        width: fit-content;
        color: #5a3e1b;
    }

    .project a {
        color: #5a3e1b;
        transition: transform 0.3s ease, filter 0.3s ease, text-shadow 0.3s ease;
        display: inline-block;
        text-decoration: none;
    }

    .project a:hover {
        transform: scale(1.1);
        filter: drop-shadow(2px 4px 6px rgba(0, 0, 0, 0.4));
        cursor: pointer;
        text-shadow: 1px 1px 2px rgba(0,0,0,0.6);
        color: #a0522d;
    }

    .links {
        text-align: center;
        margin-bottom: 40px;
    }

    .links a {
        transition: transform 0.3s ease, filter 0.3s ease, text-shadow 0.3s ease;
        display: inline-block;
        text-decoration: none;
    }

    .links a:hover {
        transform: scale(1.1);
        filter: drop-shadow(2px 4px 6px rgba(0, 0, 0, 0.4));
        cursor: pointer;
        text-shadow: 1px 1px 2px rgba(0,0,0,0.6);
    }

    .icon {
        width: 42px;
        height: 42px;
        filter: grayscale(100%) sepia(60%) hue-rotate(10deg) saturate(500%) brightness(90%);
        transition: filter 0.3s ease;
        margin: 0 10px;
    }

    .icon:hover {
        filter: none;
    }

    .centered.menu-title {
        border: 1px solid #8b4513; /* thin saddle brown border */
        padding: 16px 24px;
        margin-bottom: 50px;
        border-radius: 8px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        margin-left: auto;
        margin-right: auto;
        text-align: center;
    }

    .teck-stack-section {
        margin-top: 60px;
    }

    .subsection {
        margin-bottom: 80px;
        text-align: center;
    }

    .subsection-title {
        font-family: 'Palatino', serif;
        font-size: 32px;
        color: #8b4513;
        margin-bottom: 20px;
    }

    .language-logos {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 20px;
    }

    .language-logos img {
        width: 140px;
        height: 140px;
        margin-right: 25px;
        object-fit: contain;
        transition: filter 0.3s ease;
        cursor: default;
    }

    @keyframes bob {
        0%, 100% {
            transform: translateY(0);
        }
        50% {
            transform: translateY(-10px);
        }
    }

    .language-logos img:hover {
        filter: none;
        animation: bob 0.6s ease-in-out infinite;
    }

    .section-divider {
        border: none;
        border-top: 4px solid #d2b48c; /* tan color */
        width: 75%;
        margin-bottom: 0px;
        margin-top: -120px;
        /* margin: 10px auto; */
    }
</style>
