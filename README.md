# Hey! Welcome to my profile! :wave:

<style>
body {
  font-family: "Raleway";
  font-size: 13px/20px;
 
}

.container {
  margin: 60px 0;
  width: 400px;
  text-align: center;
}

.container .progress {
  margin: 0 ;
  width: 400px;
}

.progress {
  padding: 4px;
  background: rgba(0, 0, 0, 0.25);
  border-radius: 6px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.25), 0 1px rgba(255, 255, 255, 0.08);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.25), 0 1px rgba(255, 255, 255, 0.08);
}

.progress-bar {
  height: 16px;
  border-radius: 4px;
	background-image: -webkit-linear-gradient(top, rgba(255, 255, 255, 0.3), rgba(255, 255, 255, 0.05));
  background-image: -moz-linear-gradient(top, rgba(255, 255, 255, 0.3), rgba(255, 255, 255, 0.05));
  background-image: -o-linear-gradient(top, rgba(255, 255, 255, 0.3), rgba(255, 255, 255, 0.05));
  background-image: linear-gradient(to bottom, rgba(255, 255, 255, 0.3), rgba(255, 255, 255, 0.05));
  -webkit-transition: 0.4s linear;
  -moz-transition: 0.4s linear;
  -o-transition: 0.4s linear;
  transition: 0.4s linear;
  -webkit-transition-property: width, background-color;
  -moz-transition-property: width, background-color;
  -o-transition-property: width, background-color;
  transition-property: width, background-color;
  -webkit-box-shadow: 0 0 1px 1px rgba(0, 0, 0, 0.25), inset 0 1px rgba(255, 255, 255, 0.1);
  box-shadow: 0 0 1px 1px rgba(0, 0, 0, 0.25), inset 0 1px rgba(255, 255, 255, 0.1);
    width: 100%;
  background-color: #86e01e;
}

/*
 * Note: using adjacent or general sibling selectors combined with
 *       pseudo classes doesn't work in Safari 5.0 and Chrome 12.
 *       See this article for more info and a potential fix:
 *       https://css-tricks.com/webkit-sibling-bug/
 */

#five:checked ~ .progress > .progress-bar {
  width: 5%;
  background-color: #f63a0f;
}

#twentyfive:checked ~ .progress > .progress-bar {
  width: 25%;
  background-color: #f27011;
}

#fifty:checked ~ .progress > .progress-bar {
  width: 50%;
  background-color: #f2b01e;
}

#seventyfive:checked ~ .progress > .progress-bar {
  width: 75%;
  background-color: #f2d31b;
}

#onehundred:checked ~ .progress > .progress-bar {
  width: 100%;
  background-color: #86e01e;
}

#hideProgressBar:checked ~ .hide-on-trigger {
  display: none;
}


.radio {
  display: none;
}

.label {
  display: inline-block;
  margin: 0 5px 20px;
  padding: 3px 8px;
  color: #aaa;
  text-shadow: 0 1px black;
  border-radius: 3px;
  font-weight: 600;
}

.radio:checked + .label {
  color: white;
  background: rgba(0, 0, 0, 0.25);
}

/* About me */

.about-me {
  display: none;
}

#showAboutMe:checked ~ .about-me {
    display: inline-block;
}

</style>

<div class="container hide-on-trigger">
  <input type="radio" class="radio" name="progress" value="five" id="five">

  <input type="radio" class="radio" name="progress" value="twentyfive" id="twentyfive" checked>

  <input type="radio" class="radio" name="progress" value="fifty" id="fifty">

  <input type="radio" class="radio" name="progress" value="seventyfive" id="seventyfive">

  <input type="radio" class="radio" name="progress" value="onehundred" id="onehundred">

  <input type="radio" class="radio" name="hideProgressBar" value="hideProgressBar" id="hideProgressBar">
  <label class="label hide-on-trigger">Loading aboutMe.ts file...</label>

  <div class="progress hide-on-trigger">
    <div class="progress-bar hide-on-trigger"></div>
  </div>
</div>

<script> 
const animateBar = () => {
    setTimeout(()=> {
      document.getElementById('five').click(); 
    }, 0)

    setTimeout(()=> {
      document.getElementById('twentyfive').click(); 
    }, 1000)

    setTimeout(()=> {
      document.getElementById('fifty').click(); 
    }, 2000)

    setTimeout(()=> {
      document.getElementById('seventyfive').click(); 
    }, 3000)

    setTimeout(()=> {
      document.getElementById('onehundred').click(); 
    }, 5000)

    setTimeout(()=> {
      document.getElementById('showAboutMe').click(); 
    }, 6000)

    setTimeout(()=> {
      document.getElementById('hideProgressBar').click(); 
    }, 6000)

}
</script>

<input type="radio" class="radio" name="showAboutMe" value="showAboutMe" id="showAboutMe">
<div id='about-me' class="about-me">

```TypeScript
class About extends Me {
  constructor(
  private personalInfo: MyPersonalInformation,
  private skills: string[],
  private languages: LanguageItem[],
  ) {
  this.personalInfo = this.getPersonalInformation();
  this.skills = this.getSkills();
  this.languages = this.getLanguages();
  };

  getPersonalInformation(): MyPersonalInformation {
    const personalInformation: MyPersonalInformation = {
    firstName: "Ivan",
    middleName: "Francisco",
    lastName: "Miragaya",
    age: 22,
    currentLocation: "Buenos Aires, Argentina",
    techInterests: ['Web3', 'Ethereum', 'Cardano', 'Blockchain'];
    };

    return personalInformation;
  };

  getSkills(): string[] {
   const hardSkills: string[] = ['Microservices-architecture', 'IasS', 'SOLID enthusiast']

   const softSkills: string[] = [
        'Proactivity (seriously)',
        'Team player',
        'Communicative',
        'Troubleshooting',
        'Clean coder (clean architecture)'
        ];

    return [...hardSkills, ...softSkills];
  };

  getLanguages(): LanguageItem[] {
    return [
        {
          language: 'English',
          level: 'Professional (advanced)'
        },
        {
          language: 'Spanish',
          level: 'Native'
        }
     ];
  };
}
```

</div>

## :hammer_and_wrench: Some tools that i use

<img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/javascript/javascript-original.svg" alt="JavaScript" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/react/react-original.svg" alt="react" width="50" height="50" style="padding: 5px"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/vuejs/vuejs-original.svg" alt="Vue.js" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/nodejs/nodejs-original.svg" alt="NodeJS" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/nestjs/nestjs-plain.svg" alt="NestJS" width="25" height="25"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/express/express-original.svg" alt="express.js" width="50" height="50" style="padding: 5px; background-color: #ffffff;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/solidity/solidity-original.svg" alt="Solidity" width="50" height="50" style="padding: 5px; background-color: #ffffff;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/docker/docker-original.svg" alt="docker" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="AWS" width="50" height="50" style="padding: 5px; background-color: #ffffff;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/mysql/mysql-original.svg" alt="MySQL" width="25" height="25"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/postgresql/postgresql-original.svg" alt="postgres" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/mongodb/mongodb-original.svg" alt="MongoDB" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/jest/jest-plain.svg" alt="jest" width="50" height="50" style="padding: 5px;">

## Now learning :orange_book:

Im currently learning about cloud architecture. Taking the course from [Adrian Cantrill](https://www.linkedin.com/in/adriancantrill/) in [learn.cantrill.io](https://learn.cantrill.io/).

- Next stop :busstop: [AWS - Certified developer associate](https://aws.amazon.com/certification/certified-developer-associate/)

## Lets chat :mailbox:

<a href="https://www.linkedin.com/in/miragaya-ivan/">
<img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/linkedin/linkedin-original.svg" alt="LinkedIn" width="50" height="50" style="padding: 5px;"/>
  </a>

<a href="mailto:miragayaivan@hotmail.com">
<img src="https://www.freeiconspng.com/uploads/gmail-logo-icon-4.png" alt="Email" width="50" height="50" style="padding: 5px;"/>
  </a>

<br/>
<br/>

![Ivan's Github stats](https://github-readme-stats.vercel.app/api?username=m-ivan&show_icons=true&theme=synthwave&count_private=true)
