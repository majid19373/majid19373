<h1>š Hi, Iām Seyed Majid Attar</h1>

- š I'm skilled in javascript, Typescript, React, Next.js, Front-End.
- šļø I'm intrested in Typescript, Flutter.
- š« Contact me:  {
        email: majidsma19373@gmail.com,
        linkedin: <a href='https://www.linkedin.com/in/seyed-majid-attar-0bb57b18b' target='_blank'>seyed majid attar</a>,
        telegram: <a href='https://t.me/majid19373' target='_blank'>majid19373</a>
    }

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
            š ${this.about()}
            - š I'm skilled in ${this.skills.toString()}.
            - šļø I'm intrested in ${this.favorites.toString()}.
            - š« Contact me: ${JSON.stringify(this.contacts)}
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



<!-- - š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ... -->

<!---
majid19373/majid19373 is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
