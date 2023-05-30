# React-portfolio
## AIM:
### To create a portfolio using REACT JS.
## PROCEDURE:
### 1. Create a new react project using the following comments in command prompt:
###                   npx create-react-app file-name
### 2. After creating the project open its directoy and give the command as npm start.
### 3. Now in APP.js manupulate the required components as required
### 4. We can either create new components in the same page or create a new file and the import them.
### 5. We can also add stylesheet into REACT and make our webpage more interractive
### 6. Finally export all the components to get the output.
## PROGRAM:
### APP.js
```
import logo from './logo.svg';
import './App.css';

function App() {
  return (
    <body>
      <Header />
      <Start />
      <Career />
      <Skills />
      <Education/>
      <Contact/>
    </body>
      
  );
}
function Header(){
  return(
    <div className="header">
      <div className="header_elements">
        <a href='#career' style={{textDecoration: 'none', color: 'black'}}>
        CAREER</a>
      </div>
      <div class="header_elements"><a href="#skills" style={{textDecoration: 'none', color: 'black'}}>
        SKILLS
      </a></div>
      <div class="header_elements"><a href="#edu" style={{textDecoration: 'none', color: 'black'}}>
        Education
      </a></div>
      <div class="header_elements"><a href="#contact" style={{textDecoration: 'none', color: 'black'}}>
                Contact me</a>
      </div>
    </div>
  );
}
function  Start(){
  return(
    <div className='start'>
      
      <div style={{fontSize: 46, paddingTop: 140 ,paddingLeft: 2,paddingRight: 170, color: 'antiquewhite'}} className='start_element'><b>HELLO THERE!</b><br></br>
      THIS IS PAVITHRA 😄.<br></br> TAKE A QUICK TOUR OF<br></br> MY PORTFOLIO AND<br></br> SEE WHAT I AM CAPABLE OF! </div>
      <div className='start_element'></div>
    </div>
  );
}
function Career(){
  return (
    <div class='career' id='career'>
      <div class='career_comp'><link rel="preconnect" href="https://fonts.googleapis.com"></link>
              <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin></link>
          <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap" rel="stylesheet"></link>
          <h1 style={{textAlign: 'centre'}}><b>ABOUT CAREER</b></h1>
            Myself PAVITHRA from department of <i>ARTIFICIAL INTELLIGENCE<br></br> AND MACHINE LEARNING(AIML). </i>
            I would like to work upon<br></br> AI emerging field and very much interested in AR and VR concepts.<br></br>
            I am looking forward to improve my skills based on this field <br></br>and currently i m working on it as well.<br></br>
            I am always optimistic towords my goal and self-motivated to <br></br>achieve the targets. Hence I am looking 
            forward to work in<br></br> development field and very much interested in improving my<br></br> experience in it.
      </div>
      <div class='career_comp'>
        <img src={require('./career.jpg')} style={{height: 580, width: 550 ,borderRadius: 25}}></img>
      </div>
    </div>
  );
}
function Skills(){
  return (
    <div class='skills' id="skills"><br></br>
      <h1 style={{fontSize: 50 , color: 'antiquewhite'}}>SKILLS</h1>
      <div className='skill_display' style={{paddingLeft: 50}}>
      <div className='skill_comp'>TECHNICAL SKILLS
        <div style={{fontSize: 35, margin: 0}}>
        <ul>
        <li><i>JAVA</i></li>
        <li><i>SQL</i></li>
        <li><i>C</i></li>
        <li><i>python</i></li>
        <li><i>Snap AR</i></li>
        <li><i>Spark AR</i></li>
        <li><i>HTML,CSS, JAVAScript, REACT JS</i></li>
        </ul>
        </div>
      </div>
      <div className='skill_bg'><img src={require('./technical.png')} style={{width: '300', height: 'auto'}}></img></div>
      </div>
      <br></br>
      <div className='skill_display'>
      <div className='skill_bg'><img src={require('./connect.jpg')} style={{width: '300', height: 'auto'}}></img></div>
      <div className='skill_comp'>SOFT SKILLS
      <ul>
        <li><i>HARDWORKING</i></li>
        <li><i>HUMBLE</i></li>
        <li><i>ADAPTABLE</i></li>
        <li><i>FRIENDLY</i></li>
        <li><i>DEDICATED</i></li>
        <li><i>EMOTIONAL BALANCE</i></li>
        <li><i>TEAM WORK</i></li>
        </ul></div>
      </div>
    </div>
  );
}
function Education(){
  return(
    <div class="edu" id="edu"><h1>EDUCATION</h1>
      <div className='edu_comp'><ul>
        <li><h2>Highschool: </h2><i>SKNSPMC VIVEKANANDA VIDHYALAIYA JUNIOR COLLEGE</i></li>
      <li><h2>UG: </h2><i>SAVEETHA ENGINEERING COLLEGE</i></li>
      <li><h2>DEGREE: </h2><i>BTech.Artificial Inteliigence and Machine Learning</i></li>
      <li><h2>LANGUAGES: </h2><i>English,German,Tamil,Telugu</i></li>
      </ul>
      </div>
    </div>
  );
}
function Contact(){
  return(
    <div class='contact' id="contact">
      <div class='contact_comp'>CONTACT ME:</div>
      <div class='contact_comp'>
        <a href='pavithra0607gjm@gmail.com' ><img src="https://icons-for-free.com/download-icon-google+mail+icon-1320192249286867468_512.png" 
        style={{width: 50, height: 50}}></img></a>
      </div>
      <div class='contact_comp'>
        <a href='https://github.com/gpavithra673'><img src="https://w7.pngwing.com/pngs/914/758/png-transparent-github-social-media-compute
        r-icons-logo-android-github-logo-computer-wallpaper-banner-thumbnail.png" style={{width: 50, height: 50}}></img></a>
      </div>
      <div class='contact_comp'>
        <a href='https://www.linkedin.com/in/pavithra-g-990442237/'><img src="https://assets.stickpng.com/images/6297a2f1e01809629f113598.png" 
                        style={{width: 50, height: 50}}></img></a>
      </div>
    </div>
  );
}
export default App;

```
### Stylesheet.css
```


.start{
  
  display: flex;
  padding: 10px;
  padding-bottom: 80px;
  padding-top: 70px;
  background-image: url(./bg7.jpg);
  background-size: cover;
  justify-content: center;
}
.start_element:nth-child(even){
  width: 520px;
  text-align: center;
  height: 518px;
  padding: 25px;
  background-image: url(./profile.jpg);
  transform: translate(-80px,50px);
  background-size: cover;
  font-size: 65px;
}
.header{
  background-color:#877a6e;
  padding-top: 10px;
  padding-bottom: 10px;
  padding-left: 100px;
  display: flex;
  justify-content: flex-end;
  justify-content: space-between;
  padding-right: 15px;
}
.header_elements{

  display: inline-flex;
  font-size: 20px;
  font-weight: bold;
  border: 1px solid #2F234B;
  border-radius: 35px;
  padding: 10px;
  position: relative;
  background-color: #f7e0c7;
  color: #2F234B;
}
.header_elements:hover{
  animation: buttonup1 infinite;
  animation-duration: 0.6s;
  animation-direction:alternate;
  
}
@keyframes buttonup1 {
  from {top: 0px;}
  to {top: 10px;}
}
.career{
  padding:50px;
  height: 600px;
  width: 1358px;
  background-image: url(./bg5.jpg);
  background-size: cover;
  display:inline-flex;
  align-items: center;
}
.career_comp{
  font-family: 'Bebas Neue', sans-serif;
  font-size: 35px;
  padding: 10px;
  color: antiquewhite;
}
.skills{
  padding:50px;
  height: auto;
  width: 1358px;
  background-color: #5e5348;
  background-size: cover;
  display:inline-flexbox;
  align-content: space-around;
}
.skill_display{
  display:flex;
  padding: 20px;
  justify-content: space-around;
}
.skill_bg{
  font-family: 'Bebas Neue', sans-serif;
  display: inline-flex;
  justify-content: space-around;
  font-size: 35px;
  width: auto;
  height: 400px;
  color: rgb(7, 7, 7);
  
}
.skill_comp:nth-child(odd){
  font-family: 'Bebas Neue', sans-serif;
  display: flexbox;
  justify-content: space-around;
  font-size: 35px;
  width: 500px;
  height: 400px;
  padding: 10px;
  background-color: antiquewhite;
  color: rgb(7, 7, 7);
  border-radius: 15px;
}
.skill_comp:nth-child(even){
  font-family: 'Bebas Neue', sans-serif;
  display: flexbox;
  justify-content: space-around;
  font-size: 35px;
  width: 500px;
  height: 400px;
  padding: 10px;
  background-color: rgb(213, 245, 247);
  color: rgb(7, 7, 7);
  border-radius: 15px;
}
.edu{
  background-image: url(./bg3.jpg);
  background-size: cover;
  padding : 50px;
  font-size: 30px;
  display: flexbox;
  padding-top: 40px;
  padding-left: 550px;
  color: rgb(254, 238, 210);
}
.edu_comp{
  display: flexbox;
  font-size: 25px;
  padding: 5px;
  color: rgb(252, 241, 216);
}
.contact{
  display: flex;
  justify-content: space-around;
  background-color: #877a6e;
}
.contact_comp{
  padding: 10px;
  display: flex;
  font-size: 25px;
  color: rgb(252, 241, 216);
  border-radius: 10px;
}
```
## OUTPUT:
![Web capture_31-5-2023_11528_localhost](https://github.com/gpavithra673/React_portfolio/assets/93427264/0fa3e3d8-db05-4f26-adb7-1717677c43d2)
## RESULT:
### Hence we have successfully created a portfolio using react js.
