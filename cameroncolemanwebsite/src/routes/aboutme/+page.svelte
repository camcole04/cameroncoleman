<script>
    import brushstroke from '$lib/assets/brushstroke.png';
    import me from '$lib/assets/picofme.jpeg';
</script>

<div class="page-box">
    <h1 class="menu-title">About Me</h1>
    <div class="portrait" style="background-image: url({ me });"></div>
    <h3 class="header"> 
        <br><br/>Hey! My name is 
        <span style="color: blue; margin-bottom: -60px">
            <div class="section-title-background" style="background-image: url({ brushstroke }); margin-bottom: -40px">
            Cameron Coleman
            </div>
        </span>
        <br><br/>
        I am a motivated <span style="color: green">Software Engineer</span> with a passion for developing products that can improve the lives of others.
        <br><br/><br><br/>
    </h3>
    
    <h2 class="description"> As a 4th year Software Engineering major at the
        Rochester Institute of Technology, I am constantly looking to improve my understanding of various fields of computer software. 
        My particular <span style="color:brown">areas of interest</span> include Embedded Systems, Front End Development, and Database Management.
        <br><br/>
        I would love for my skills and strengths to be utilized on projects that will benefit society. 
        I believe technology has the ability to assist in or solve many problems humanity has created for itself and the planet.
        My goal is to use the knowledge and skills I have gained to contribute in solving these problems.
        <br><br/>
    </h2>

    <div class="header" style="margin-bottom: -100px">
        <br><br/>
        <div class="section-title-background" style="background-image: url({ brushstroke });">
        SKILLS
        </div>
        <br><br/>
    </div>

    <h2 class="description"> 
        My primary skills include <span style="color: brown">Front End Development</span> such as HTML, JavaScript, Svelte, REACT, Boot/Reactstrap among others.
        <br><br/>
        <span style="color: brown">Embedded Systems</span> with a specialty in Embedded C and some MIPS Assembly experience.
        Most of my experience for embedded programming has been with STMCube32 IDE on a NUCLEO-L476RG board.
        <br><br/>
        As well as <span style="color: brown">Database Management</span>, specifically in SQL. I have developed multiple projects using PostgreSQL including fullstack applications.
        I am currently developing a hotel management application using MySQL.
        <br><br/>
    </h2>

    <div class="header" style="margin-bottom: -100px">
        <br><br/>
        <div class="section-title-background" style="background-image: url({ brushstroke });">
        INTERESTS 
        </div>
        <br><br/>
    </div>

    <h2 class="description"> 
        My favorite hobbies are Rock Climbing, Skateboarding, and Cooking. I took inspiration from dinner menus to design this website!
        <br><br/>
        In my free time I like to read and play video games. My favorite book is House of Leaves by Mark Z. Danielewski and I can't really pin down my favorite video game.
        <br><br/>
        
    </h2>


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

    .portrait {
        border-radius: 90%;
        position: relative;
        display: flex;
        justify-content: center;
        margin: 0px auto 10px auto;
        align-items: center;
        padding: 175px 100px 100px 0px;
        background-size: 302px 403px;
        background-repeat: no-repeat;
        background-position: 50% 60%;
        max-width: 200px;
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

    .header {
        margin: auto;
        display: flex;
        flex-direction: column;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 48px;
        margin-top: -40px;
        width: fit-content;
        text-align: center;
        width: 70%
    }

    .description {
        margin: auto;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 28px;
        margin-top: -40px;
        width: 90%;
        text-align: center;
    }

    



</style>