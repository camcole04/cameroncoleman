<div class="centered">
    <div class="page-box">
        <h1 class="menu-title">Midi Audio Microcontroller</h1>
        <h3 class="header">
            Designed software to control playback of songs stored in the MIDI format. Controls include: Next, Play, Pause, and Stop. Changes between remote (terminal) and local (button) control modes.
            <br/><br/>
            Gained experience with microcontroller programming, memory and CPU architecture, communication interfaces, and applying software development best practices including testing and ethical considerations for safety-critical systems.
        </h3>

        <div class="media-placeholders">
            <div class="image-placeholder">
                <p>Image of the device will go here</p>
            </div>
            <div class="video-placeholder">
                <p>Video of the device will go here</p>
            </div>
        </div>
    </div>
</div>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Alegreya+Sans&display=swap');
    @import '$lib/styles.css';

    .section-title-background {
        display: inline-block;
        padding: 35px 55px;
        padding-right: 40px;
        background-repeat: no-repeat;
        background-size: 100% 90%; 
        background-position: center;
        text-align: center;
    }

    .menu-title {
        margin: 0 auto;
        text-align: center;
        background-color: #FF70A6;
        border-radius: 20px;
        border: 6px solid #E9FF70;
        margin-top: 50px;
        margin-bottom: 50px;
        padding: 40px;
        font-size: 60px;
        width: fit-content;
        box-shadow: 0 0 20px 20px #E9FF70;
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
        margin-top: -40px;
        text-align: center;
        line-height: 1.5;
    }

    .media-placeholders {
        display: flex;
        justify-content: center;
        gap: 50px;
        margin-top: 50px;
        flex-wrap: wrap;
    }

    .image-placeholder, .video-placeholder {
        border: 3px dashed #FF70A6;
        border-radius: 15px;
        width: 300px;
        height: 200px;
        display: flex;
        justify-content: center;
        align-items: center;
        font-family: Arial, sans-serif;
        font-size: 18px;
        color: #FF70A6;
        background-color: #fff0f5;
        text-align: center;
        padding: 10px;
    }
</style>
