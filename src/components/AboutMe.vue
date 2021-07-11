<template>
    <div class="about-me">
        <p>My interest in tech started when I was a child, I would write small programs, 
            like password protection programs on my Commodore Plus 4.
            However, as an adult I pursued a career in the ambulance service, where I gained
            some valuable skills, such as how to build a rapport with people quite quickly, 
            and how to convey important information clearly and concisely.
            <br><br>
            However, for several year now I have dreamt of following my interest in tech,
            which is why four years ago I decided to undertake a BSc (Hons) degree with 
            The Open University to gain the qualifications necessary to pursue a career change.
            <br><br>
             In doing so I have rediscovered my passion for coding, and have found that because I 
            enjoy it so much I learn new coding skills quickly and easily. Furthermore, I am able 
            to think logically when trying to overcome problems involving code, and have the resilience
            and perseverance to not give up until the problem is solved.
            <br><br>
            Despite having no professional experience in the field, I am hard working and motivated 
            to become a professional developer.
        </p>
        <br><br>
        <h3>My top skills</h3>
        <br>


        <div class="grid-container">

            <div class="grid-item">
                <div class="skills-title">
                    <i class="fa fa-star" aria-hidden="true"></i>
                    <h4>HTML</h4>
                </div>
                <div class="skills-content">
                    <p>
                        I have been using HTML for some time now and feel that I am quite 
                        competant in this technology.
                    </p>
                </div> 

            </div>

            <div class="grid-item">
                <div class="skills-title">
                    <i class="fa fa-star" aria-hidden="true"></i>
                    <h4>CSS</h4>
                </div>
                <div class="skills-content">
                    <p>
                        As with HTML, I have been practising CSS for some time and am
                         competent in this technology. I would however like to learn a 
                         CSS pre-processing language such as SASS.
                    </p>
                </div>

            </div>

            <div class="grid-item">
                <div class="skills-title">
                    <i class="fa fa-star" aria-hidden="true"></i>
                    <h4>JavaScript</h4>
                </div>
                <div class="skills-content">
                    <p>
                        I have been practising vanilla JavaScript for just a few years.
                        I have created a few personal projects and feel comfortable with the syntax.
                    </p>
                </div>

            </div>

            <div class="grid-item">
                <div class="skills-title">
                    <i class="fa fa-star" aria-hidden="true"></i>
                    <h4>CCNA</h4>
                </div>
                <div class="skills-content">
                    <p>
                        I have recently studied for the CCNA (Cisco Certified Network Associate) with The Open University.
                        I am competant in network troubleshooting and fault finding.
                    </p>
                </div>

            </div>

        </div>

        
    </div>
</template>

<script>
export default{
    name: 'AboutMe',    
}

</script>

<style>
    .about-me{
        margin-top: 40px;
        width: 600px;
        float: left;
        font-size: 20px;
    }

    .fa{
        color: white;
        background-color: #34796C;
        border-radius: 50px;
        padding: 5px;
        margin-right: 10px;
    }

    .top-row{
        display: inline-flex;
        flex-direction: row;
        width: 100%;
        justify-content: space-between;

    }

    .bottom-row{
        margin-top: 50px;
        display: inline-flex;
        flex-direction: row;
        width: 100%;        
        justify-content: space-between;
    }

    .skills-title{
        display: inline-flex;
        font-size: 24px;
    }


    .skills-content{
        margin-left: 45px;
    }

    .grid-container {
        display: grid;
        grid-template-columns: auto auto;
        padding: 10px;
    }

    .grid-item {
        padding: 20px;
        text-align: left;
    }
</style>