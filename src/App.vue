<template>
  <div class="main" id="main">
      <header>
        <title>
          Sid portofolio
        </title> 
      </header>
      <div class="topbar">
          <a href="https://www.instagram.com/sidvaneijndhoven/" id="topAnimation">
            ©SidvanEijndhoven
          </a>
      </div>
      <div class="nav">
          <nav>
          <ul>
            <li>
              <a href="#main">Home</a>
            </li>
            <li>
              <a href="#projecten">Projecten</a> 
            </li>
            <li>
              <a href="#stage">Stage</a>
            </li>
          </ul>
        </nav>
      </div>
      <div class="sidebar">
        <div class="me">
            <img src="./assets/photo2.png" class="me">
        </div>
        <p>Sid<br> van <br> Eijndhoven<br></p>
        <h2>
          Socials:
        </h2>
        <p>
          GitHub:
        </p>
        <a href="https://github.com/Sidvaneijndhoven/Projecten">
          <img id="github" src="./assets/github.png">
        </a>
        <p>
          LinkedIn:
        </p>
        <a href="https://www.linkedin.com/in/sid-van-eijndhoven-02167a302/">
          <img src="./assets/linkedin.webp" id="linkedin">
        </a>
        <p>
          Mijn CV:
        </p>
        <button>
          <a href="./assets/CvSid (1).pdf" download>Download CV</a>
        </button>
        <div id="progress-bar"></div>
      </div>
      <div class="home">
        <h1 class="welcome">
          <span id="welcomeSpan">Welkom!</span> Mijn naam is Sid van Eijndhoven<br> en ik doe de opleiding Software Developer!
        </h1>
        <div class="banner">
          <div class="text">
            <img src="./assets/stars-background.png" id="meBanner">
              <h2>
                  Over Mij
              </h2>
              <p>
                Momenteel zit ik in leerjaar 2 op het Koning Willem I college in Den Bosch.<br>
                In mijn vrije tijd doe ik gamen en verzorg ik mijn luipaardgekko Draco.<br>
                Mijn favoriete spel op dit moment is: ©Call Of Duty BO6.<br>
                Daarnaast heb ik een bijbaantje bij de Albert Heijn in Boxtel als vakkenvuller.
              </p>
          </div>        
        </div>    
        <div class="hobby">
          <h2>
            Hobby's
          </h2>
          <img src="./assets/draco.webp" id="pet">
          <img src="./assets/setup.webp" id="setup">
        </div>
      </div>
      <div class="stage" id="stage">
        <h2>
          Stage
        </h2>
        <img src="./assets/protix_logo_4.png" id="logoProtix">
        <p>
          Protix(03-09-2024 - 31-01-2025)<br>
          Ik heb bij Protix stage gelopen samen met Anthony en het software team.<br>
          Heb ik Cypress front end testen gemaakt voor hun applicatie Entosoft.<br>
          Ik heb ook eigen projectjes gemaakt met: Python, C#, vue3 en Cypress <br>om te kijken hoe het is om met diversen talen te werken.
        </p>
      </div>
      <div class="projects" id="projecten">
        <h2>
          Projecten
        </h2>
        <p>
          voorbeelden van mijn projecten
        </p>
        <div class="examples">
          <p>Kleine Python scriptjes:</p>
          <img src="./assets/code1.webp" class="python1" id="left1">
          <img src="./assets/code2.webp" class="python1" id="center2">
          <img src="./assets/code3.webp" class="python1" id="right3">
          <p>Cypress testen:</p>
          <video autoplay loop class="video1" id="vid">
            <source src="./assets/user_entosoft.feature.mp4" type="video/mp4">
          </video>
          <p>
            Hierin wordt getest of een user met breed acces een sbu kan starten<br> 
            en daarna wordt er met een Read Only<br> account ingelogd om te kijken of de stop batch button bestaat.<br>
            Deze test is ook gemaakt met Cypress Cucumber!
          </p>
          <video autoplay loop class="video2" id="vid">
            <source src="./assets/Cypress pokemon generator test.mp4" type="video/mp4">
          </video>
          <p>
            Hierin wordt een Pokemon api getest met alle pokemons<br> erin om te kijken of de api stabiel is en werkt.
          </p>
          <video autoplay loop class="video3" id="vid">
            <source src="./assets/Country-guide api tests how it looks in cypress.mp4" type="video/mp4">
          </video>
          <p>
            Hierin wordt een country flag api getest<br> met alle vlaggen om te kijken of de api stabiel is en werkt
          </p>
          <video autoplay loop class="video4" id="vid">
            <source src="./assets/workinstr_entosoft.feature.mp4" type="video/mp4">
          </video>
          <img src="./assets/discord-log.png" class="dcLog" id="vid">
          <img src="./assets/wi_img.png" class="wiImg" id="vid">
          <p class="cypressLog">
            Cypress X Cucumber + Discord Log<br>
            Cypress cucumber test alle rode en gele expired work instructions worden gelogt naar mijn Discord server.
          </p>
          <h2>
            Cypress Cucumber🥒
          </h2>
          <img src="./assets/Cucumber-user.png" class="cucumberUser" id="Img">
        </div>
      </div>
  </div>
</template>
<script>
export default{}
import { animate, inView } from "motion";
import { nextTick } from 'vue';

nextTick(() => {
  // Animations with delays
  animate("li", { x: -100 });  
  setTimeout(() => {
    animate(".topbar", { x: [500, 0], duration: 2, ease: "ease-in-out" });
  }, 1000);  
  
  setTimeout(() => {
    animate(".sidebar", { y: [500, 0], duration: 2, ease: "ease-in-out" });
  }, 1500);  
  
  setTimeout(() => {
    animate("#github", { transform: ["rotate(0deg)", "rotate(360deg)"], duration: 40, ease: "ease-in-out" });
  }, 5000);  

  setTimeout(() => {
    animate("#linkedin", { transform: ["rotate(0deg)", "rotate(360deg)"], duration: 40, ease: "ease-in-out" });
  }, 5000);  
  
  setTimeout(() => {
    animate("#meBanner", { x: [2000, 0], duration: 2, ease: "ease-in-out" });
  }, 3000);  
  
  setTimeout(() => {
    animate(".me", { x: [-200, 0], duration: 2, ease: "ease-in-out" });
  }, 2500); 

  inView("#pet", (info) => {
  const animation = animate(info.target, {
    y: [600, 0],
    duration: 1,
    easing: "ease-out"
  });

  return () => {
    animation.stop();  
  };
});

//inviews:
inView("#setup", (info2) => {
  const animation2 = animate(info2.target, {
    y: [-600, 0],
    duration: 1,
    easing: "ease-out"
  });

  return () => {
    animation2.stop(); 
  };
});

inView("#logoProtix", (info3) => {
  animate(info3.target, {
    x: [-600, 0],
    duration: 1,
    easing: "ease-out"
  });
});

inView("#left1", (info4) => {
  const animation4 = animate(info4.target, {
    x: [-400, 0],
    duration: 1,
    easing: "ease-in-out"
  });

  return () => {
    animation4.stop(); 
  };
});

inView("#center2", (info5) => {
  const animation5 = animate(info5.target, {
    y: [-400, 0],
    duration: 1,
    easing: "ease-in-out"
  });

  return () => {
    animation5.stop(); 
  };
});

inView("#right3", (info6) => {
  const animation6 = animate(info6.target, {
    x: [400, 0],
    duration: 1,
    easing: "ease-in-out"
  });

  return () => {
    animation6.stop(); 
  };
});

inView("#vid", (info7) => {
   animate(info7.target, {
    x: [400, 0],
    duration: 1,
    easing: "ease-in-out"
  });
});

inView("#Img", (info7) => {
   animate(info7.target, {
    y: [400, 0],
    duration: 1,
    easing: "ease-in-out"
  });
});

//progress bar 
const progressBar = document.getElementById('progress-bar');

const updateProgress = () => {
  const scrollPosition = window.scrollY;
  const pageHeight = document.documentElement.scrollHeight - window.innerHeight;
  const progress = (scrollPosition / pageHeight) * 100;

  animate(progressBar, {
    height: `${progress}%`,
  }, {
    duration: 0.1,
  });
};

window.addEventListener('scroll', updateProgress);
updateProgress()
})

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body
{
  background: linear-gradient(to right, rgb(14, 14, 42), rgb(0, 0, 0));
  text-align: center;
  color: white;
  font-family: Cambria;
  margin: 0px;
  overflow-x: hidden;
}

li  
{
  margin-top: 50px;
  margin-right: 60px;
  list-style-type: none;
  display: inline-flex;
  float: right;
}

ul
{
  margin: 0px;
}

a
{
  position: relative;
  text-decoration: none;
  color: white;
  font-size: 25px;
}

li a:hover
{
  background-color: rgb(58, 59, 59);
  color: black;
}

.sidebar
{
  width: 12vw;
  height: 1000vh;
  position: relative;
  padding-bottom: 1000px;
  float: left;
  background: linear-gradient(to top left, #808080, #222222);
  box-shadow: 2px 2px #222222;
  color: white;
  font-family: monospace;
  font-size: 20px;
  text-align: center;
}

.topbar 
{
  height: 5vh;
  width: 100vw;
  background: linear-gradient(to left, #808080, #333333);
  margin: 0px;
  box-shadow: 2px 2px #222222;
  position: relative;
  overflow: hidden;
}

#topAnimation 
{
  position: absolute;
  left: -100%;
  margin: 0px;
  font-size: 20px;
  padding-top: 3px;
  white-space: nowrap;
  animation: slideIn 20s linear infinite;
}

.home 
{
  color: white;
  text-align: center;
}

.welcome 
{
  width: 0;
  height: 150px; 
  position: relative;
  font-family: monospace;
  margin: 33vh auto 0px auto;
  font-size: 24px;
  white-space: nowrap;
  overflow: hidden;
  animation: typing 10s steps(400) 2s forwards;
}

#welcomeSpan
{
  font-size: 30px;
  animation: colorChange 8s infinite alternate;
}

.me 
{
  width: 7vw;
  height: auto;
  position: relative;
  margin: 3vh auto 0px auto;
  border-radius: 60%; 
}

#github
{
  width: 7vw;
  height: auto;
  position: relative;
  margin: 0px auto 0px auto;
  cursor: pointer;
}

#linkedin
{
  width: 7vw;
  height: auto;
  position: relative;
  margin: 0px auto 0px auto;
  cursor: pointer;
}

button
{
  width: auto;
  height: auto;
  position: relative;
  border-radius: 15px;
  margin: 0px auto 0px auto;
  background-color: rgb(51, 51, 212);
  padding: 8px 10px;
  border: none;
  box-shadow: 1px 1px rgb(73, 73, 231);
}

button a:hover
{
  color: black;
}

button a
{
  font-size: 15px;
  font-family: monospace;
}

#meBanner
{
  position: relative;
  width: 86vw;
  height: 75vh;
  opacity: 5;
  border: 3px solid black;
  float: left;
  margin: 100px auto 75px auto;
}

.text
{
  position: relative;
  width: auto;
  height: auto;
  text-align: center;
  color: white;
}

.text h2 
{
  position: absolute;
  width: auto;
  height: auto;
  top: 150px;
  font-family: monospace;
  font-size: 30px;
  left: 50%;
  transform: translate(-50%, -50%);
}

.text p 
{
  position: absolute;
  width: auto;
  height: auto;
  top: 270px;
  font-family: monospace;
  font-size: 20px;
  left: 50%; 
  transform: translate(-50%, -50%);
}

#pet, #setup
{
  width: auto;
  height: 70vh;
  position: relative;
  margin: 0px auto 0px auto;
  border-radius: 25px;
  opacity: 0.5;
  animation: boxShadow 3s infinite ease-in-out;
}

#pet:hover
{
  width: auto;
  height: 73vh;
  opacity: 5;
  cursor: default;
}

#setup:hover
{
  width: auto;
  height: 73vh;
  opacity: 5;
  cursor: default;
}

#setup
{
  margin-left: 20px;
}

.stage h2
{
  color: white;
  font-family: monospace;
  font-size: 30px;
}

.stage
{
  margin-top: 300px;
  color: white;
  font-family: monospace;
  font-size: 20px;
}

#logoProtix
{
  width: 10vw;
  height: auto;
  position: relative;
  margin: 0px auto 0px auto;
}

.projects
{
  margin-top: 300px;
  color: white;
  font-family: monospace;
  font-size: 20px;
}
.python1
{
  width: 20vw;
  height: auto;
  position: relative;
  margin: 0px 20px 0px auto;
  display: inline-flex;
  opacity: 0.5;
}

.python1:hover
{
  opacity: 5;
  width: 22vw;
  height: auto;
}

.video1, .video2, .video3
{
  width: 50vw;
  border-radius: 15px;
  height: auto;
  position: relative;
  margin: 100px auto 0px auto;
  animation: boxShadow 3s infinite ease-in-out;
}

.video4
{
  width: 40vw;
  border-radius: 15px;
  height: auto;
  float: left;
  position: relative;
  margin: 100px auto 0px 40px;
  animation: boxShadow 3s infinite ease-in-out;
}

.dcLog
{
  width: 40vw;
  border-radius: 15px;
  height: auto;
  float: right;
  position: relative;
  margin: 100px 40px 0px auto;
  animation: boxShadow 3s infinite ease-in-out;
}

#progress-bar 
{
  position: absolute;
  top: 0;
  left: 0;
  width: 5px;
  height: 0; 
  background-color: rgb(85, 139, 255)
}

.wiImg
{
  width: 40vw;
  border-radius: 15px;
  height: auto;
  position: relative;
  margin: 20px 10px 0px 20px;
  animation: boxShadow 3s infinite ease-in-out;
}

.cucumberUser
{
  width: 60vw;
  border-radius: 15px;
  height: auto;
  position: relative;
  margin: 20px 10px 0px 20px;
  animation: boxShadow 3s infinite ease-in-out;
}

/* Other animation */
@keyframes rotate
{
  from
  {
    rotate: 0deg;
  }

  to
  {
    rotate: 360deg;
  }
}
@keyframes typing 
{
  from {
    width: 0;
  }
  to {
    width: 100%;
    overflow: visible;
  }
}

@keyframes colorChange {
    0% {
        color: #FF5733; 
    }
    25% {
        color: #33FF57;
    }
    50% {
        color: #3357FF; 
    }
    75% {
        color: #F3FF33; 
    }
    100% {
        color: #FF5733; 
    }
}

@keyframes slideIn 
{
  0% {
    left: -100%;
    color: #FF5733;
  }
  50% {
    left: 50%;
    transform: translateX(-50%);
    color: #33FF57;
  }
  100% {
    left: 100%;
    color: #3357FF; 
  }
}

@keyframes boxShadow
{
  from 
  {
    box-shadow: 2px 2px #2575c4;
  }

  to 
  {
  box-shadow :2px 2px #2c3e50;
  }
}

/* Responsive */

@media only screen and (max-width: 426px)
{
  body
  {
    width: 100vw;
  }

  .sidebar
  {
    height: 100vh;
    width: 25vw;
    font-size: 15px;
    padding: 5px 10px;
  }

  .sidebar h2
  {
    font-size: 25px;
  }

  .nav
  {
    width: auto;
    height: auto;
    margin: 100px auto 200px 150px;
    display: flex;
  }

  .nav a 
  {
    font-size: 25px;
    font-family: monospace;
  }

  .me
  {
    width: 25vw;
    height: auto;
  }

  .welcome, #welcomeSpan
  {
    font-size: 17px;
    overflow: visible;
    white-space: normal;
    display: inline-block;

  }

  #github, #linkedin
  {
    width: 30vw;
    height: auto;
  }

  .text p
  {
    position: absolute;
    width: auto;
    height: auto;
    top: 550px;
    font-family: monospace;
    font-size: 17px;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  #pet, #setup
  {
    width: 80vw;
    height: auto;
    margin: 0px auto 100px auto;
  }

  #logoProtix
  {
    width: 60vw;
    margin: 0px auto 0px auto;
  }

  .video1, .video2, .video3
  {
    width: 80vw;
    height: auto;
    margin: 0px auto 0px auto;
  }

  .video4
  {
    margin-left: 50px;
    width: 80vw;
    height: auto;
  }

  .dcLog, .wiImg
  {
    width: 80vw;
    height: auto;
    margin: 20px auto 20px auto
  }

  .cucumberUser
  {
    width: 80vw;
    height: auto;
    margin-bottom: 200px;
  }

  .dcLog
  {
    margin-right: 50px;
  }
}

@media only screen and (max-width: 376px)
{
  body
  {
    width: 100vw;
  }

  .sidebar
  {
    height: 100vh;
    width: 25vw;
    font-size: 15px;
    padding: 5px 10px;
  }

  .sidebar h2
  {
    font-size: 25px;
  }

  .nav
  {
    width: auto;
    height: auto;
    margin: 100px auto 200px 150px;
    display: flex;
  }

  .nav a 
  {
    font-size: 25px;
    font-family: monospace;
  }

  .me
  {
    width: 25vw;
    height: auto;
  }

  .welcome, #welcomeSpan
  {
    font-size: 17px;
    overflow: visible;
    white-space: normal;
    display: inline-block;

  }

  #github, #linkedin
  {
    width: 30vw;
    height: auto;
  }

  .text p
  {
    position: absolute;
    width: auto;
    height: auto;
    top: 550px;
    font-family: monospace;
    font-size: 17px;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  #pet, #setup
  {
    width: 80vw;
    height: auto;
    margin: 0px auto 100px auto;
  }

  #logoProtix
  {
    width: 60vw;
    margin: 0px auto 0px auto;
  }

  .video1, .video2, .video3
  {
    width: 80vw;
    height: auto;
    margin: 0px auto 0px auto;
  }

  .video4
  {
    margin-left: 50px;
    width: 80vw;
    height: auto;
  }

  .dcLog, .wiImg
  {
    width: 80vw;
    height: auto;
    margin: 20px auto 20px auto
  }

  .cucumberUser
  {
    width: 80vw;
    height: auto;
  }

  .dcLog
  {
    margin-right: 20px;
  }
}

@media only screen and (max-width: 321px)
{
  body
  {
    width: 100vw;
  }

  .sidebar
  {
    height: 100vh;
    width: 25vw;
    font-size: 15px;
    padding: 5px 10px;
  }

  .sidebar h2
  {
    font-size: 20px;
  }

  .nav
  {
    width: auto;
    height: auto;
    margin: 100px auto 200px 150px;
    display: flex;
  }

  .nav a 
  {
    font-size: 30px;
    font-family: monospace;
  }

  .me
  {
    width: 25vw;
    height: auto;
  }

  .welcome, #welcomeSpan
  {
    font-size: 20px;
    overflow: visible;
    white-space: normal;
    display: inline-block;
  }

  #github, #linkedin
  {
    width: 30vw;
    height: auto;
  }

  .text p
  {
    position: absolute;
    width: auto;
    height: auto;
    top: 550px;
    font-family: monospace;
    font-size: 20px;
    left: 50%;
    transform: translate(-50%, -50%);
  }

  #pet, #setup
  {
    width: 80vw;
    height: auto;
    margin: 0px auto 100px auto;
  }

  #logoProtix
  {
    width: 60vw;
    margin: 0px auto 0px auto;
  }

  .video1, .video2, .video3
  {
    width: 80vw;
    height: auto;
    margin: 0px auto 0px auto;
  }

  .video4
  {
    margin-left: 50px;
    width: 80vw;
    height: auto;
  }

  .dcLog, .wiImg
  {
    width: 80vw;
    height: auto;
    margin: 20px auto 20px auto
  }

  .cucumberUser
  {
    width: 80vw;
    height: auto;
  }

  .dcLog
  {
    margin-right: 20px;
  }
  

}

</style>

