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
