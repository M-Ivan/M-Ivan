### Hi there 👋



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



<!--
**M-Ivan/m-ivan** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
## Some tools that i use

<img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/javascript/javascript-original.svg" alt="JavaScript" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/react/react-original.svg" alt="react" width="50" height="50" style="padding: 5px"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/vuejs/vuejs-original.svg" alt="Vue.js" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/nodejs/nodejs-original.svg" alt="NodeJS" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/nestjs/nestjs-plain.svg" alt="NestJS" width="25" height="25"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/express/express-original.svg" alt="express.js" width="50" height="50" style="padding: 5px; background-color: #ffffff;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/solidity/solidity-original.svg" alt="Solidity" width="50" height="50" style="padding: 5px; background-color: #ffffff;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/docker/docker-original.svg" alt="docker" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="AWS" width="50" height="50" style="padding: 5px; background-color: #ffffff;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/mysql/mysql-original.svg" alt="MySQL" width="25" height="25"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/postgresql/postgresql-original.svg" alt="postgres" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/mongodb/mongodb-original.svg" alt="MongoDB" width="50" height="50" style="padding: 5px;"><img src="https://raw.githubusercontent.com/devicons/devicon/1119b9f84c0290e0f0b38982099a2bd027a48bf1/icons/jest/jest-plain.svg" alt="jest" width="50" height="50" style="padding: 5px;">

