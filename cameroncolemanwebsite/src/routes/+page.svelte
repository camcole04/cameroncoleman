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
        
        <p class="section-title"><a href="/aboutme">ABOUT ME </a> </p>
        
        <div class="section-title-background" style="background-image: url({ brushstroke });">
            <p class="section-title">PROJECTS </p>
        </div>
        <p class="project"><a href="/projects/midiaudioplayer">Midi Audio Player</a> </p>

        <!-- New Teck Stack Section -->
        <div class="teck-stack-section">
            <p class="section-title">Tech Stack</p>
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
                </div>
            </div>
            <div class="subsection">
                <p class="subsection-title">Frameworks</p>
                <!-- Frameworks later -->
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
        /* margin-bottom: 30px; */
        font-style: italic;
    }

    .section-title {
        margin: auto;
        font-family: 'Palatino', serif;
        margin-bottom: 30px;
        font-size: 48px;
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

    .section-title-background {
        position: relative;
        display: flex;
        justify-content: center;
        margin-bottom: 40px;
        align-items: center;
        padding-top: 10px; 
        background-size: 350px 90px;
        background-repeat: no-repeat;
        background-position: 50%;
    }

    .section-title-background:hover {
        filter: sepia(1) hue-rotate(10deg) brightness(0.8);
        cursor: pointer;
    }

    .project {
        margin: auto;
        font-family: 'Palatino', serif;
        font-size: 24px;
        margin-top: -40px;
        width: fit-content;
        color: #5a3e1b;
    }

    .project a {
        color: #5a3e1b;
        text-decoration: none;
        border-bottom: 1px dotted #8b4513;
    }

    .project a:hover {
        color: #a0522d;
        border-bottom: 1px solid #a0522d;
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

    /* New styles for Teck Stack section */
    .teck-stack-section {
        margin-top: 60px;
    }

    .subsection {
        margin-bottom: 40px;
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
        width: 128px;
        height: 128px;
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
</style>
