# Resume-Portfolio

----------Index-------------
<!DOCTYPE html>
<html lang="eg"> 
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width,initial-scale=1.0">
    <title>Poonam Resume Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <script src="https://kit.fontawesome.com/934b3727c7.js" crossorigin="anonymous"></script>
</head>
<body>

  -----------------header----------------------
    <div id="header">
        <div class="container">
            <nav>
                <img src="images/Logo.png" height="50" width="1000" class="logo">
                <ul id="sidemenu">
                    <li><a href="#header">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#contact">Contact</a></li>
                    <i class="fa-solid fa-xmark" onclick="closemenu()"></i>
                </ul>
                <i class="fa-solid fa-bars" onclick="openmenu()"></i>
            </nav>
            <div class="header-text">
                <p>Frontend Developer</p>
                <h1>Hello, I'm <span>Poonam Shinde</span> <br>from Aurangabad</h1>
            </div>
        </div>
    </div>
    
<!----------About---------->
<div id="about">
    <div class="container">
        <div class="row">
            <div class="about-col-1">
                <img src="images/Poonam.jpg">
            </div>
            <div class="about-col-2">
                <h1 class="sub-title">About Me</h1>
                <p>Experienced Full Stack Developer with One years of expertise in designing, 
                    developing, and deploying webapplications. Proficient in front-end and 
                    back-end technologies, with a strong foundation in softwareengineering 
                    principles</p>

                    <div class="tab-titles">
                        <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
                        <p class="tab-links" onclick="opentab('experience')">Experience</p>
                        <p class="tab-links" onclick="opentab('education')">Education</p>
                    </div>
                    <div class="tab-contents active-tab" id="skills">
                        <ul>
                            <li><span>Full Stack Development</span><br>designing Front-end and Back-end Interface</li>
                            <li><span>Web Development</span><br>Desiging webApplication Development</li>
                            <li><span>App Development</span><br>Building Android/ios app</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="experience">
                        <ul>
                            <li><span>Full Stack Development</span><br>Full Stack Development Training at M.C. Talent Hunt</li>
                            <li><span>2023-2024</span><br>internship at ActioHX</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="education">
                        <ul>
                            <li><span>2023</span><br>Full Stack Development At M.C. Talent Hunt</li>
                            <li><span>2023</span><br>M.SC(IT) From Aurangabad</li>
                            <li><span>2021</span><br>B.Sc(CS) From Aurangabad</li>
                        </ul>
                    </div>
            </div>
        </div>
    </div>
</div>

<!--------Projects----------->
<div id="projects">
    <div class="container">
        <h1 class="sub-title">MY Projects</h1>
        <div class="projects-list">
            <div class="projects">
                <img src="images/Camera.jpg">
                <div class="layer">
                <h3>Photography Management System(2023)</h3>
                <p>Description:A Web Application for Book any 
                    photoshoot like Portrait, Marraige, Maternity, NewBorn Baby 
                    Technologies used: HTML5, CSS3, JavaScript</p>
                <a href="https://github.com/poonam015/Photography_WebSite"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
            </div>
        </div>

        <div class="projects">
            <img src="images/Online shopping.jpg">
            <div class="layer">
            <h3>Online Shoppy Management System(2023)</h3>
            <p>Description: Shop online mobile and handle there data
                Technologies used: Spring Boot, MySql</p>
            <a href="https://github.com/poonam015/Online_Shoppy"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
        </div>
    </div>

    <div class="projects">
        <img src="images/Students.jpg">
        <div class="layer">
        <h3>Student Management System(2023)</h3>
        <p>Description: Here i used the Mapping Methods
            Technologies used: Hibernate</p>
        <a href="https://github.com/poonam015/Photography_WebSite"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
    </div>
</div>
</div>
<a href="#" class="btn">See More</a>
    </div>
</div>

<!-------------Contact------------>
<div id="contact">
    <div class="Container">
        <div class="row">
            <div class="contact-left">
                <h1 class="sub-title">Contact Me</h1>
                <p><i class="fa-solid fa-paper-plane"></i>poonamshinde15628@gmail.com</p>
                <p><i class="fa-solid fa-square-phone"></i>123456789</p>
                <div class="social-icons">
                    <a href="https://github.com/poonam015"><i class="fa-brands fa-github"></i></a>
                    <a href="https://www.facebook.com/"><i class="fa-brands fa-facebook"></i></a>
                    <a href="https://x.com/i/flow/login"><i class="fa-brands fa-twitter"></i></a>
                    <a href="https://www.linkedin.com/in/poonam-shinde-15r/"><i class="fa-brands fa-linkedin"></i></a>
                </div>
                <a href="images/Poonam Shinde (Full Stack Developer) (1).pdf" download class="btn btn2">Download Rsume</a>
            </div>
            <div class="contact-right">
                <form name="submit-to-google-sheet">
                    <input type="text" name="Name" placeholder="Your Name" required>
                    <input type="email" name="Email" placeholder="Your Email" required>
                    <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
                    <button type="submit" class="btn btn2">Submit</button>
                </form>
                <span id="msg"></span>
            </div>
        </div>
    </div>
    <div class="copyright">
        <p>copyright @Poonam Shinde Resume</p>
    </div>
</div>
            
<script>

    var tablinks = document.getElementsByClassName("tab-links");
    var tabcontents = document.getElementsByClassName("tab-contents");

    function opentab(tabname){
        for(tablink of tablinks){
            tablink.classList.remove("active-link");
        }
        for(tabcontent of tabcontents){
            tabcontent.classList.remove("active-tab");
        }
        event.currentTarget.classList.add('active-link');
        document.getElementById(tabname).classList.add("active-tab");
    }

</script>

<script>
    var sidemenu = document.getElementById("sidemenu");

    function openmenu(){
        sidemenu.style.right = "0";
    }
    function closemenu(){
        sidemenu.style.right = "-200px";
    }
</script>

<script>
    const scriptURL = 'https://script.google.com/macros/s/AKfycbzgThG6KwlMku3E8l9xkDwmbU5czKfcMmsFjsQVTa11GmNUBE33ZOMw3HNZGQPnVgwf/exec'
    const form = document.forms['submit-to-google-sheet']
    const msg = document.getElementById("msg")
  
    form.addEventListener('submit', e => {
      e.preventDefault()
      fetch(scriptURL, { method: 'POST', body: new FormData(form)})
        .then(response => {
            msg.innerHTML = "Message Send Succefully"
            setTimeout(function(){
                msg.innerHTML = ""
            },5000)
            form.reset()
        })
        .catch(error => console.error('Error!', error.message))
    })
  </script>

</body>


</html>

------------------css style--------------

*{
    margin: 0;
    padding: 0;
    font-family: 'poppins', sans-serif;
    box-sizing: border-box;
}
html{
    scroll-behavior: smooth;
}
body{
    background: #10062d;
    color: #fff;
}
#header {
    width: 100%;
    height: 100vh;
    background-size: cover;
    background-position: center;
}
.container{
    padding: 10px 10%;
}
nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}

.logo{
    width: 500px;
}

nav ul li{
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
}

nav ul li a{
    color: #db71c0;
    text-decoration: none;
    font-size: 18px;
    position: relative;
}

nav ul li a::after{
    content: '';
    width: 0;
    height: 3px;
    background: #c71b79;
    position: absolute;
    left:0;
    bottom: -6px;
    transition: 0.5s;
}

nav ul li a:hover::after{
    width: 100%;
}
.header-text{
    margin-top: 20%;
    font-size: 30px;
    color: #0ae0f3;
}
.header-text h1{
    font-size: 60px;
    margin-top: 20px;
}
.header-text h1{
    color: #c71b79;
}

/*-----------About---------*/
#about{
    padding: 80px 0;
    color: #ababab;
}
.row{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.about-col-1{
    flex-basis: 35%;
}
.about-col-1 img{
    width: 100%;
    border-radius: 15px;
}
.about-col-2{
    flex-basis: 60%;
}

.sub-title{
    font-size: 60px;
    font-weight: 600;
    color: #ababab;
}
.tab-titles{
    display: flex;
    margin: 20px 0 40px;
}
.tab-links{
    margin-right: 50px;
    font-size: 18px;
    font-weight: 500;
    cursor: pointer;
    position: relative;
}
.tab-links::after{
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition: 0.5s;
}
.tab-links.active-link::after{
    width: 50%;
}
.tab-contents ul li{
    list-style: none;
    margin: 10px 0;
}
.tab-contents ul li span{
    color: #b54769;
    font-size: 14px;
}
.tab-contents{
    display: none;
}
.tab-contents.active-tab{
    display: block;
}

/*-------------Portfolio----------------*/
#projects{
    padding: 50px 0;
}
.projects-list{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}
.projects{
    border-radius: 10px;
    position: relative;
    overflow: hidden;
}
.projects img{
    width: 100%;
    border-radius: 10px;
    display: flex;
    transition: transform 0.5s;
}
.layer{
    width: 100%;
    height: 0;
    background: linear-gradient(rgba(0,0,0,0.6), #ff004f);
    border-radius: 10px;
    position: absolute;
    left: 0;
    bottom: 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 0 40px;
    text-align: center;
    font-size: 14px;
    transition: height 0.5s;
}
.layer h3{
    font-weight: 500;
    margin-bottom: 20px;
}
.layer a{
    margin-top: 20px;
    color: #ff004f;
    text-decoration: none;
    font-size: 18px;
    line-height: 60px;
    background: #2633f0;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    text-align: center;
}
.projects:hover img{
    transform: scale(1.1);
}
.projects:hover .layer{
    height: 100%
}
.btn{
    display: block;
    margin: 50px auto;
    width:fit-content;
    border: 1px solid #ff004f;
    padding: 14px 50px;
    border-radius: 6px;
    text-decoration: none;
    color: #fff;
    transition: background 0.5s;
}
.btn:hover{
    background: #ff004f;
}

/*-----------Contact---------*/
.contact-left{
    flex-basis: 35%;
}
.contact-right{
    flex-basis: 60%; 
}
.contact-left p{
    margin-top: 30px;
}
.contact-left p i{
    color: #11e7e7;
    margin-right: 15px;
    font-size: 25px;
}
.social-icons{
    margin-top: 30px;
}
.social-icons a{
    text-decoration: none;
    font-size: 30px;
    margin-right: 15px;
    color: #ababab;
    display: inline-block;
    transition: transform 0.5s;
}
.social-icons a:hover{
    color: #39ebdf;
    transform: translateY(-5px);
}
.btn.btn2{
    display: inline-block;
    background: #eb0a86;
}
.contact-right form{
    width: 100%;
}
form input, form textarea{
    width: 100%;
    border: 0;
    outline: none;
    background: #262626;
    padding: 15px;
    margin: 15px;
    color:#fff;
    font-size: 18px;
    border-radius: 6px;
}
form btn2{
    padding: 14px 60px;
    font-size: 18px;
    margin-top: 20px;
    cursor: pointer;
}
.copyright{
    width: 100%;
    text-align: center;
    padding: 25px 0;
    background: #262626;
    font-weight: 300;
    margin-top: 20px;
}

/*------------css for small screen-------*/
nav .fa-solid{
    display: none;
}

@media only screen and (max-width: 600px){
    .header-text{
        margin-top: 100%;
        font-size: 16px;
    }
    .header-text h1{
        font-size: 30px;
    }
    nav .fa{
        display: block;
        font-size: 25px;
    }
    nav ul{
        background: #19e9f8;
        position: fixed;
        top: 0;
        right: -200;
        width: 200px;
        height: 100vh;
        padding-top: 50px;
        z-index: 2; 
        transition: right 0.5s;
    }
    nav ul li{
        display: block;
        margin: 25px;
    }
    nav ul .fa{
        position: absolute;
        top: 25px;
        left: 25px;
        cursor: pointer;
    }
    .sub-title{
        font-size: 40px;
    }
    .about-col-1, .about-col-2{
        flex-basis: 100%;
    }
    .about-col-1{
        margin-bottom: 30px;
    }
    .about-col-2{
        font-size: 14px;
    }
    .tab-links{
        font-size: 16px;
        margin-right: 20px;
    }
    .contact-left, .contact-right{
        flex-basis: 100%;
    }
    .copyright{
        font-size: 14px;
    }
}
#msg{
    color: #61b752;
    margin-top: -40px;
    display: block;
}
    

