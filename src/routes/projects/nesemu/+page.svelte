<script>
    import githublogo from '$lib/assets/githublogo.png';
</script>

<div class="centered">
    <div class="page-box">
        <h1 class="menu-title">Text/Image Crypto Device (Full Stack)</h1>
        <div class="icon-container">
            <a href="https://github.com/camcole04/nes65emu">
                <img 
                    src={githublogo}
                    class="icon"
                    alt="Cameron's GitHub">
                Check Out The Git!
            </a>
        </div>
        <hr class="section-divider">
        <h3 class="header">
            Developing a custom NES emulator in Rust by implementing a 6502 CPU, memory bus, and opcode execution pipeline from the ground up. Gained hands-on experience with low-level systems programming, memory management, CPU architecture, and modular Rust design
            <br/><br/>
        </h3>
    </div>
</div>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Alegreya+Sans&display=swap');
    @import '$lib/styles.css';

    .icon {
        width: 42px;
        height: 42px;
        filter: grayscale(100%) sepia(60%) hue-rotate(10deg) saturate(500%) brightness(90%);
        transition: filter 0.3s ease;
        margin-bottom: -8px;
    }

    .menu-title {
        color: #8b4513; /* saddle brown */
        margin: 0 auto;
        text-align: center;
        margin-top: 50px;
        font-size: 60px;
        width: fit-content;
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

    .header {
        margin: auto;
        display: flex;
        flex-direction: column;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 28px;
        text-align: center;
        line-height: 1.5;
    }


    .section-divider {
        border: none;
        border-top: 4px solid #d2b48c; /* tan color */
        width: 75%;
        margin: 10px auto;
        margin-bottom: 50px;
    }

    .icon-container {
        display: flex;
        justify-content: center;
        max-width: fit-content;
        margin: auto;
        font-size: 30px;
        font-family: 'Palatino', serif;
        border: 3px solid #8b4513; /* saddle brown */
        border-radius: 10px;
        background-color: #d2b48c;
        padding: 5px;
        margin-top: 10px;
    }
</style>
