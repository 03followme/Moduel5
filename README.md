# Moduel5
Module5
// Object representing a fictional dog from animated television
let myDog = {
    name: "Astro",
    breed: "Great Dane",
    color: "Brown",
    owner: "The Jetson family",
    cartoon: "The Jetsons",
    mySound: "I sound very lovable and friendly, just like my happy bark!"
};

// Displaying the dog's information to the user
console.log(`Meet ${myDog.name} from ${myDog.cartoon}. ${myDog.name} is a ${myDog.color} ${myDog.breed} owned by ${myDog.owner}. ${myDog.name} says, "${myDog.mySound}"`);

// Dog constructor function
function Dog(name, breed, color, owner, cartoon, mySound, canTalk) {
    this.name = name;
    this.breed = breed;
    this.color = color;
    this.owner = owner;
    this.cartoon = cartoon;
    this.mySound = mySound;
    this.canTalk = canTalk;
    
    // Method to display greeting
    this.myGreeting = function() {
        if (this.canTalk) {
            console.log(`Hello! I'm ${this.name} from ${this.cartoon}. I'm a ${this.color} ${this.breed} owned by ${this.owner}. ${this.mySound}`);
        } else {
            console.log(`Hello! I'm ${this.name} from ${this.cartoon}. I'm a ${this.color} ${this.breed} owned by ${this.owner}. Sorry, I can't talk.`);
        }
    };
}

// Creating a new dog object using the constructor
let myDogConst = new Dog("Astro", "Great Dane", "Brown", "The Jetson family", "The Jetsons", "I sound very lovable and friendly, just like my happy bark!", true);

// Calling the method to display the greeting
myDogConst.myGreeting();
