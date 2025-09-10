# 👋 Hi there, I'm Majid Attar

## 🚀 Full Stack Developer & Software Architecture Enthusiast

Welcome to my GitHub! I'm a passionate **Full Stack Developer** with 5+ years of experience building robust, scalable applications. I love crafting clean code and designing elegant software architectures that solve real-world problems.

### 💻 Tech Stack & Expertise

**Backend Development**
- **PHP & Laravel** - Building enterprise-level web applications
- **Database Technologies** - MySQL, PostgreSQL, MongoDB
- **Currently Learning** - Golang for high-performance microservices

**Frontend Development**
- **React.js** - Creating dynamic, responsive user interfaces
- **Next.js** - Full-stack React applications with SSR/SSG
- **TypeScript** - Type-safe JavaScript development

**Software Architecture & Design**
- 🏗️ **Domain Driven Design (DDD)** - Currently mastering
- 🔧 **Clean Architecture** - Building maintainable systems
- 🔀 **Microservices** - Designing distributed architectures
- 📐 **Design Patterns** - Applying proven solutions to common problems

### 🌱 Currently Learning

I'm constantly evolving and expanding my skill set:

- **Golang** - Exploring Go's simplicity and performance for backend services
- **Domain Driven Design** - Deep diving into strategic and tactical patterns
- **Clean Architecture** - Implementing Uncle Bob's architectural principles
- **Microservices Architecture** - Building scalable, distributed systems
- **Advanced Design Patterns** - GoF patterns and modern architectural patterns

### 🎯 What I'm Passionate About

- 🏛️ **Software Architecture** - Designing systems that scale and evolve
- 🔄 **Clean Code** - Writing maintainable, testable, and readable code
- 📊 **Database Design** - Crafting efficient data models and queries
- 🚀 **Performance Optimization** - Making applications fast and responsive
- 🧠 **Problem Solving** - Tackling complex technical challenges

### 📈 GitHub Stats

![Your GitHub stats](https://github-readme-stats.vercel.app/api?username=your-username&show_icons=true&theme=radical)

### 🛠️ Languages & Tools

![PHP](https://img.shields.io/badge/-PHP-777BB4?style=flat-square&logo=php&logoColor=white)
![Laravel](https://img.shields.io/badge/-Laravel-FF2D20?style=flat-square&logo=laravel&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white)
![Go](https://img.shields.io/badge/-Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)


### 🤝 Let's Connect

I'm always excited to collaborate on interesting projects or discuss software architecture!

- 💼 **LinkedIn**: <a href='https://www.linkedin.com/in/majid19373' target='_blank'>majid19373</a>
- 📧 **Email**: <a href='mailto:majidsma19373@gmail.com' target='_blank'>majidsma19373@gmail.com</a>
---

⭐️ From [majid19373](https://github.com/majid19373)

``` go
package main

import (
	"fmt"
	"strings"
	"time"
)

type Developer struct {
	Name              string
	Title             string
	Experience        int
	BackendSkills     []string
	FrontendSkills    []string
	Databases         []string
	CurrentlyLearning []string
	Passions          []string
}

func NewDeveloper() *Developer {
	return &Developer{
		Name:       "Majid Attar",
		Title:      "Full Stack Developer & Software Architecture Enthusiast",
		Experience: 5,
		BackendSkills: []string{
			"PHP", "Laravel", "Golang (Learning)",
		},
		FrontendSkills: []string{
			"React.js", "Next.js", "TypeScript", "JavaScript",
		},
		Databases: []string{
			"MySQL", "PostgreSQL", "MongoDB",
		},
		CurrentlyLearning: []string{
			"Golang", "Domain Driven Design (DDD)",
			"Clean Architecture", "Microservices", "Design Patterns",
		},
		Passions: []string{
			"Software Architecture", "Clean Code", "Problem Solving",
			"Performance Optimization", "Scalable Systems",
		},
	}
}

func (d *Developer) Introduce() {
	fmt.Println("🚀 " + strings.Repeat("=", 60) + " 🚀")
	fmt.Printf("       Welcome! I'm %s\n", d.Name)
	fmt.Println("🚀 " + strings.Repeat("=", 60) + " 🚀")
	fmt.Println()

	d.showBasicInfo()
	d.showTechStack()
	d.showLearningJourney()
	d.showPassions()
}

func (d *Developer) showBasicInfo() {
	fmt.Println("👨‍💻 PROFILE OVERVIEW")
	fmt.Println(strings.Repeat("-", 40))
	fmt.Printf("🎯 Title: %s\n", d.Title)
	fmt.Printf("⏳ Experience: %d+ years in Full Stack Development\n", d.Experience)
	fmt.Printf("💡 Focus: Building scalable, maintainable software solutions\n")
	fmt.Println()
}

func (d *Developer) showTechStack() {
	fmt.Println("🛠️  TECHNICAL EXPERTISE")
	fmt.Println(strings.Repeat("-", 40))

	fmt.Println("🔧 Backend Technologies:")
	for _, skill := range d.BackendSkills {
		fmt.Printf("   • %s\n", skill)
	}

	fmt.Println("\n🎨 Frontend Technologies:")
	for _, skill := range d.FrontendSkills {
		fmt.Printf("   • %s\n", skill)
	}

	fmt.Println("\n🗄️  Database Technologies:")
	for _, db := range d.Databases {
		fmt.Printf("   • %s\n", db)
	}
	fmt.Println()
}

func (d *Developer) showLearningJourney() {
	fmt.Println("📚 CURRENT LEARNING JOURNEY")
	fmt.Println(strings.Repeat("-", 40))
	fmt.Println("🌱 Actively expanding knowledge in:")
	for _, topic := range d.CurrentlyLearning {
		fmt.Printf("   • %s\n", topic)
	}
	fmt.Println()
}

func (d *Developer) showPassions() {
	fmt.Println("❤️  WHAT DRIVES ME")
	fmt.Println(strings.Repeat("-", 40))
	for _, passion := range d.Passions {
		fmt.Printf("   🔥 %s\n", passion)
	}
	fmt.Println()
}

func (d *Developer) AnimatedIntro() {
	messages := []string{
		"🚀 Initializing developer profile...",
		"💻 Loading technical expertise...",
		"🧠 Processing architectural knowledge...",
		"✅ Ready to code and collaborate!",
	}

	for _, message := range messages {
		fmt.Println(message)
		time.Sleep(800 * time.Millisecond)
	}
	fmt.Println()
}

func main() {
	developer := NewDeveloper()

	developer.AnimatedIntro()

	developer.Introduce()
}

