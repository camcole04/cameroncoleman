<div class="centered">
    <div class="page-box">
        <h1 class="menu-title">Ultrasonic Note Recognition Game</h1>
        <hr class="section-divider">
        <h3 class="header">
            Developed a device that plays a certain note based on the distance an object is from the ultrasonic sensor.
            The user can choose between some hard coded songs and what octave they want to play at.
            A single light within a row of lights will light up to represent the next note in the song.
            The objective for the user is to play all the notes of the song as accurately as possible.
            The device contains a red light, blue light, and a green light that activates when the user is too close, too far, or correct respectively.
            <br/><br/>
            Gained experience with microcontroller sensor programming.
        </h3>

        <div class="media-placeholders">
            <div class="image-placeholder">
                <p>Image of the device will go here</p>
            </div>
            <div class="video-placeholder">
                <p>Video of the device will go here I real</p>
            </div>
        </div>
    </div>
</div>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Alegreya+Sans&display=swap');
    @import '$lib/styles.css';

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

    .section-divider {
        border: none;
        border-top: 4px solid #d2b48c; /* tan color */
        width: 75%;
        margin: 10px auto;
        margin-bottom: 50px;
    }
</style>
