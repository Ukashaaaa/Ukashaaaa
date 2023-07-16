// 2
let person: string = "Eric"


let message: string = `Hello ${person}, would you like to learn some Python today?`


console.log(message)

// 3 =======================================================================================================
let person2: string = "Eric"

let lowercaseName: string = person2.toLowerCase()

let uppercaseName: string = person2.toUpperCase()

let titlecaseName: string = person2.split(" ").map((l: string) => l[0].toUpperCase() + l.substr(1)).join(" ")


console.log("Lowercase name:", lowercaseName)

console.log("Uppercase name:", uppercaseName)

console.log("Title case name:", titlecaseName)

// 4 =============================================================================================
let quote: string = "A person who never made a mistake never tried anything new."

let author: string = "Albert Einstein"


console.log(`${author} once said, "${quote}"`)

// 5 ==========================================================================================
let quote2: string = "A person who never made a mistake never tried anything new."

let famousPerson: string = "Albert Einstein"

let message2: string = `${famousPerson} once said, "${quote2}"`

console.log(message2)

// 6 =======================================================================================
let nameWithWhitespace: string = "\t\n   John Doe   \t\n"

console.log("Name with whitespace:", nameWithWhitespace)


let strippedName: string = nameWithWhitespace.trim()

console.log("Stripped name:", strippedName)

// 7 ======================================================================================
console.log("Addition:", 6 + 2)

console.log("Subtraction:", 14 - 6)

console.log("Multiplication:", 4 * 2)

console.log("Division:", 64 / 8)

// 9 =========================================================================================
let favoriteNumber: number = 42

let message3: string = `My favorite number is ${favoriteNumber}.`

console.log(message3)

// 10 ========================================================================================

// This program converts a temperature from Celsius to Fahrenheit

let celsius: number = 25

let fahrenheit: number = (celsius * 9/5) + 32


console.log(`${celsius}`)

console.log(`${fahrenheit}`)

// This program calculates the length of a string and prints the result.

let inputString: string = "Hello, World!"

let length2: number = inputString.length

console.log(`${length2}`)

// 11 ================================================================================================
let names: string[] = ["Ukasha", "Amy", "Usman", "Saim"]

for (let i = 0; i < names.length; i++) {

  console.log(names[i])


  let personalizedMessage: string = message.replace("{name}", names[i])


  console.log(personalizedMessage)
}

//13 =============================================================================================
let favoriteTransportation = ["motorcycle"]

console.log(`I would love to own Honda ${favoriteTransportation}`)

// 14 ==================================================================================================
let guestList = ["Albert Einstein", "Elon Musk", "Zack"]

for (let i = 0; i < guestList.length; i++) {

  let guest = guestList[i]

  console.log(`Dear ${guest}, you are invited to dinner. I would love to preserve you`)
}

// 15 ==================================================================================================
let guestCannotMakeIt = "Elon Musk"
let newGuest: string = "Billie Elish"

console.log(`Unfortunately, ${guestCannotMakeIt} cannot make it to dinner.`)

guestList.splice(guestList.indexOf(guestCannotMakeIt), 1)

guestList.push(newGuest)

for (let i = 0; i < guestList.length; i++) {

  let guest = guestList[i]


  console.log(`Dear ${guest}, you are invited to dinner. I would love to preserve you.`)
}
// 16 =======================================================================================================

console.log("Good news! We found a bigger dinner table.")

guestList.unshift("Rutther Ford") // begining or array
guestList.splice(Math.floor(guestList.length / 2), 0, "Isaac Newton") // Middle of Array
guestList.push("Jane Austen") // End of the array

for (let i = 0; i < guestList.length; i++) {
  let guest = guestList[i];
  console.log(`Dear ${guest}, you are invited to dinner. I would love to preserve you.`);
}

// 17 =======================================================================================================
console.log("Oops! The new dinner table won't arrive in time. We can only invite two people for dinner.")

while (guestList.length > 2) {

  let removedGuest = guestList.pop()


  console.log(`Sorry, ${removedGuest}, we can't invite you to dinner.`)
}

for (let i = 0; i < guestList.length; i++) {

  let guest = guestList[i]

  console.log(`Dear ${guest}, you are still invited to dinner. We apologize for the change in plans.`)
}

guestList = [] 

console.log("Final guest list:", guestList)

// 18 ===============================================================================================
let placesToVisit = ["Makkah", "Madina", "Malaysia", "Germeny", "Paris"]


console.log("Original order:", placesToVisit)


let sortedAlphabetically = [...placesToVisit].sort()

console.log("Alphabetical order:", sortedAlphabetically)

console.log("Original order:", placesToVisit);

let sortedReverseAlphabetically = [...placesToVisit].sort().reverse()

console.log("Reverse alphabetical order:", sortedReverseAlphabetically)


console.log("Original order:", placesToVisit)


placesToVisit.reverse()
console.log("Reversed order:", placesToVisit)


placesToVisit.reverse()
console.log("Original order:", placesToVisit)


placesToVisit.sort()
console.log("Alphabetical order:", placesToVisit)


placesToVisit.sort().reverse()
console.log("Reverse alphabetical order:", placesToVisit)

// 19 ==============================================================================================
console.log(`The number of people invited to dinner is ${guestList.length}.`)

// 20============================================================================================
let landmarks = [
    "Faisal Mosque",
    "Dhani Waterfall",
    "Monument",
    "Badshahi Masjid"
    
  ]

  
  console.log("List of Famous Landmarks:")

  for (let i = 0; i < landmarks.length; i++)  {

    console.log(landmarks[i])

  }

// 21 ======================================================================================
let book1 = {
    title: "Arabian Sea",
    author: "Amma Watson",
    year: 2000,
    genre: "Classic",
  }
  
  let book2 = {
    title: "2005",
    author: "Nawaz Sharif",
    year: 2010,
    genre: "Fiction",
  }
  
  let book3 = {
    title: "The Great Man",
    author: "Imran Khan",
    year: 2020,
    genre: "Classic",
  }
  
  
  let bookList = [book1, book2, book3];
  

  for (let i = 0; i < bookList.length; i++) {

    let book = bookList[i]

    console.log(`Title: ${book.title}`)

    console.log(`Author: ${book.author}`)

    console.log(`Year: ${book.year}`)

    console.log(`Genre: ${book.genre}`)

  }
  
  // 22======================================================================================
  let numbers = [1, 2, 3, 4, 5]

  console.log(numbers[15]) //index error

  console.log(numbers[5]); // valid index

  // 23 =================================================================================
  let car = 'subaru'

console.log("Is car == 'subaru'? I predict true.")
console.log(car == 'subaru')

console.log("Is car == '5 wheeler'? I predict false.")
console.log(car == '5 wheeler')

console.log("Is car != 'Kia'? I predict true.")
console.log(car != 'Kia')

console.log("Is car != 'subaru'? I predict false.")
console.log(car != 'subaru')

console.log("Is car === 'subaru'? I predict true.")
console.log(car === 'subaru')

console.log("Is car === 'honda'? I predict false.")
console.log(car === 'honda')

console.log("Is car !== 'ford'? I predict true.")
console.log(car !== 'ford')

console.log("Is car !== 'subaru'? I predict false.")
console.log(car !== 'subaru')

console.log("Is car.length > 5? I predict false.")
console.log(car.length > 5)

console.log("Is car.length < 10? I predict true.")
console.log(car.length < 10)

// 24 ==========================================================================================
let string1 = 'Hello'
let string2 = 'World'

let number1 = 5
let number2 = 10

let array = [1, 2, 3, 4, 5]

console.log("Equality test (string):")

console.log(string1 == 'Hello')      // True
console.log(string1 == string2)     // False


console.log("Inequality test (string):")

console.log(string1 != 'Goodbye')         // True
console.log(string1 != string2)          // True


console.log("Lowercase function test:")

console.log(string1.toLowerCase() == 'hello')        // True
console.log(string2.toLowerCase() == 'WORLD')       // False


console.log("Numerical tests:")

console.log(number1 == 5)                // True
console.log(number1 == number2)         // False
console.log(number1 > 3)               // True
console.log(number1 < number2)        // True
console.log(number1 >= 5)            // True
console.log(number1 <= number2)     // True


console.log("Logical operator tests:")

console.log(number1 > 3 && number2 < 15)      // True
console.log(number1 > 10 || number2 > 15)    // False


console.log("Array tests:")

console.log(3 in array)       // True
console.log(6 in array)      // False


console.log("Item not in array test:")

console.log(!array.includes(6))         // True
console.log(!array.includes(3))        // False

// 25 =================================================================================================

let alien_color = 'green'

if (alien_color === 'green') {

  console.log("Congratulations! You just earned 5 points.")

}

let alien_color2 = 'red'

if (alien_color2 === 'green') {

  console.log("Congratulations! You just earned 5 points.")

}

// 26 =====================================================================================================

let alien_color3 = 'green'

if (alien_color3 === 'green') {

  console.log("Congratulations! You just earned 5 points for shooting the alien.")

} else {

  console.log("Congratulations! You just earned 10 points.")

}

let alien_color4 = 'red'

if (alien_color4 === 'green') {

  console.log("Congratulations! You just earned 5 points for shooting the alien.")

} else {
  console.log("Congratulations! You just earned 10 points.")
}

// 27 ======================================================================================================

let alien_color5 = 'green'

if (alien_color5 === 'green') {

  console.log("Congratulations! You just earned 5 points.")

} else if (alien_color5 === 'yellow') {

  console.log("Congratulations! You just earned 10 points.")

} else if (alien_color5 === 'red') {

  console.log("Congratulations! You just earned 15 points.")

}


let alien_color6 = 'yellow'

if (alien_color6 === 'green') {

  console.log("Congratulations! You just earned 5 points.")

} else if (alien_color6 === 'yellow') {

  console.log("Congratulations! You just earned 10 points.")

} else if (alien_color6 === 'red') {

  console.log("Congratulations! You just earned 15 points.")

}


let alien_color7 = 'red'

if (alien_color7 === 'green') {

  console.log("Congratulations! You just earned 5 points.")

} else if (alien_color7 === 'yellow') {

  console.log("Congratulations! You just earned 10 points.")

} else if (alien_color7 === 'red') {

  console.log("Congratulations! You just earned 15 points.")

}

// 28 ==================================================================================================

let age = 30;

if (age < 2) {
  console.log("The person is a baby.")
 }

  else if (age < 4) {
  console.log("The person is a toddler.")
 }

  else if (age < 13) {
  console.log("The person is a kid.")
 }

  else if (age < 20) {
  console.log("The person is a teenager.")
 }

  else if (age < 65) {
  console.log("The person is an adult.")
 }

  else {
  console.log("The person is an elder.");
 }

 // 29 ======================================================================================================

 let favorite_fruits = ['banana', 'apple', 'mango'];

if (favorite_fruits.includes('banana')) {
  console.log("You really like bananas!")
}

if (favorite_fruits.includes('apple')) {
  console.log("You really like apples!")
}

if (favorite_fruits.includes('mango')) {
  console.log("You really like mangoes!")
}

if (favorite_fruits.includes('strawberry')) {
  console.log("You really like strawberries!")
}

if (favorite_fruits.includes('grape')) {
  console.log("You really like grapes!")
}

// 30 ==========================================================================================================

let usernames = ['admin', 'Ukasha', 'Saim', 'Danyal', 'Sarah']

for (let username of usernames) {
  if (username === 'admin') 
  
  {
    console.log("Hello admin, would you like to see a status report?")
  } else
  
  {
    console.log(`Hello ${username}, thank you for logging in again.`)
  }
}

// 31 ========================================================================================================

usernames = [] // Removing all usernames from the array

if (usernames.length === 0) {

  console.log("We need to find some users!")

}

// 32 =========================================================================================================

let current_users = ['admin', 'Ukasha', 'Saim', 'CR7', 'Sarah'];
let new_users = ['Ahmed', 'Ukasha', 'Akash', 'Amy', 'sarah'];

for (let new_username of new_users) {

  let usernameExists = current_users.some((current_username) =>
    current_username.toLowerCase() === new_username.toLowerCase()
  )


  if (usernameExists) {

    console.log(`Sorry, the username '${new_username}' is already taken. Please enter a new username.`)

  } else {
    console.log(`Congratulations! The username '${new_username}' is available.`)
  }
}


// 33 ========================================================================================================

let numbers1 = [1, 2, 3, 4, 5, 6, 7, 8, 9];

for (let numbers1 of numbers) {
  let ordinalNumber;
  
  if (number1 === 1) {
    ordinalNumber = '1st'


  } else if (number1 === 2) {
    ordinalNumber = '2nd'


  } else if (number1 === 3) {
    ordinalNumber = '3rd'


  } else {
    ordinalNumber = `${number1}th`
  }
  
  console.log(ordinalNumber)
}

//34 ================================================================================================

let favoritePizzas = ['Pepperoni', 'Margherita', 'Hawaiian']

for (let pizza of favoritePizzas) {

  console.log(`I like ${pizza} pizza.`)

}


console.log("I really love pizza!")

// 35 ======================================================================================================

let animals = ['dog', 'cat', 'rabbit']

for (let animal of animals) {

  console.log(`A ${animal} would make a great pet.`)

}

console.log("Any of these animals would make a great pet!")

// 36 ===========================================================================================================

function make_shirt(size: string, message: string) {

    console.log(`Size: ${size}`)
    console.log(`Message: ${message}`)

  }
  
  make_shirt("Large", "Hello World!")

  // 37 ========================================================================================================

  function make_shirt1(size = "Large", message = "I love TypeScript") {

    console.log(`Size: ${size}`)
    console.log(`Message: ${message}`)

  }
  
  make_shirt1()
  make_shirt1("Medium")
  make_shirt1("Small", "Hello, world!")

  // 38 ===============================================================================================

  function describe_city(city: string, country = "Pakistan") {

    console.log(`${city} is in ${country}.`)

  }
  
  describe_city("Karachi")
  describe_city("London", "United Kingdom")
  describe_city("Sydney", "Australia")
  
  
  // 39 =========================================================================================================

  function city_country(city: string, country: string): string {

    return `${city}, ${country}`

  }
  
  console.log(city_country("Lahore", "Pakistan"))
  console.log(city_country("Paris", "France"))
  console.log(city_country("Tokyo", "Japan"))

  // =========================================================================================================


  
