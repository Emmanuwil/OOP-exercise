# OOP-exercise
console.log("Hello World!\n==========\n");

// Exercise 1 Section
console.log("EXERCISE 1:\n==========\n");


class Person {
    constructor(name, pets, residence, hobbies) {
        this.name = name;
        this.pets = pets;
        this.residence = residence;
        this.hobbies = hobbies;
    }

    info() {
        let listHobbies = this.hobbies;
        console.log(
            `I am ${this.name}. I have ${this.pets} pets. I live in ${this.residence}. I like ${this.hobbies}.`
            );
    }

    greeting() {
        console.log("Whats Up Everyone!");
    }
}

class Coder extends Person {
    constructor(name, pets, residence, hobbies) {
        super(name, pets, residence, hobbies);
        this.occupation = "Full Stack Web Developer";
        }

    greeting() {
        console.log("Hello World " + "My name is " + this.name + "I'm a coder!")
    }
}


const Emmanuwil = new Person("Emmanuwil", 0, "Raliegh", ["Day Trading ", "coding ", "HVAC"]);

console.log(Emmanuwil); 

Emmanuwil.info()
Emmanuwil.greeting()
Emmanuwil.occupation = "Full Stack Wec Deveoper";
