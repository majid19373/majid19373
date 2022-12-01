<h1>👋 Hi, I’m Seyed Majid Attar</h1>

```yaml
type Contacts = {
    email: string
    linkedin: string
    telegram: string
}

type User = {
    name: string
    yearOfBirth: number
    skills: string[]
    favorites: string[]
    contacts: Contacts
}

class Pesron {
    protected name: string
    protected yearOfBirth: number

    constructor( name: string, yearOfBirth: number ) {
        this.name = name
        this.yearOfBirth = yearOfBirth
    }

    public about(): string {
        return `Hello, I'm ${this.name} and I was born in ${this.yearOfBirth}.`
    }

}

class Developer extends Pesron {
    private skills: string[]
    private favorites: string[]
    private contacts: Contacts

    constructor( { name, yearOfBirth, skills, favorites, contacts }: User ) {
        super( name, yearOfBirth )
        this.skills = skills
        this.favorites = favorites
        this.contacts = contacts
    }

    public printInformation():void {
        const str: string = `
            - 👀 ${this.about()}
            - 🌱 I'm skilled in ${this.skills.toString()}.
            - 💞️ I'm intrested in ${this.favorites.toString()}.
            - 📫 Contact me: ${JSON.stringify(this.contacts)}
        `
        console.log(str)
    }
}

const user: User = {
    name: 'Seyed Majid Attar',
    yearOfBirth: 1994,
    skills: ['javascript', 'Typescript', 'React', 'Next.js', 'Front-End'],
    favorites: ['Typescript', 'Flutter'],
    contacts: {
        email: 'majidsma19373@gmail.com',
        linkedin: 'seyed majid attar',
        telegram: 'majid19373'
    }
}

const developer:Developer =  new Developer({...user})
developer.printInformation()
```



<!-- - 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ... -->

<!---
majid19373/majid19373 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
