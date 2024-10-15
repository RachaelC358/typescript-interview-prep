//Explicit types:
const foo:string = "FOO";

const age:number = 12;

const isActive:boolean = false;

//object with properties
const user: {id: number; name: string}= {id: 1, name: 'Jack'};

const users: { id: number; name: string} []= [user];

// What is the difference between explicit and implicit types?

let fooo = "fooo";

const getFullName = (name: string, surname: string): string => 
  name + " " + surname;

  interface User {
    id: number;
    name: string;
}

const user: User = { id: 1, name: 'Gabby'};

const getName = (user: {id:number; name: string})=>{
  return user.name;  
};

const getName2 = (user: User)=>{
    return user.name;  
  };

getName({id: 1, name: "Shelby"});

getName(1); // typescript unhappy with types given to it because they don't match the interface

// What is a type in typescript?

//Types are data types assinged to variables
type ID = string;

const id: ID = "1";

interface User2 {
    id: number
    name: string
}

type Numbers = number[];
type user = User[];
let baa:any;

const numbers: Numbers = [1,2,3];

// What is the difference between a type and an interface.

// TypeScript adds a typing system to Javascipt, so you could access any property anywhere in your code
// In Javacript there are no types by default
// In javascript you can access a property that does not exist on an object
// TypeScript solves the problem of types in TypeScript
// TypeScript is developed by Microsoft
// Its harder to make a bug involving types if you are strongly tpying inputs and outputs of your functions
// TypeScript uses red squiggly lines to find errors in your development environment


// What is a generic function in typescript?
// Generic functions can work with multiple types and still provide some type safety.
// The type parameter acts as a placeholder for the acutal type
function identity<T>(arg: T): T {
    return arg;
}

let result1 = identity<string>("Hello");
console.log(result1); // Output: Hello

let result2 = identity<number>(42);
console.log(result2); // Output: 42



const result = myNewFunction<number>("string");
