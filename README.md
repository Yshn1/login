# login
Object Oriented JavaScript
var customer = {
name: ‘Tom Smith’,
speak: function(){
return “My name is ” + this.name;
},
address: {
street: ‘123 Main St’,
city: ‘Pittsburgh’,
state: ‘PA’
}
};
document.write(customer.speak()+ “
“);
document.write(customer.name + ” lives at ” + customer.address.street + “
“);
customer.address.country = “US”;
document.write(customer.address.country + “
“);
function Person(name, street) {
this.name = name;
this.street = street;
this.info = function(){
return “My name is ” + this.name + ” and I live on ” + this.street;
}
}
var bobSmith = new Person(“Bob Smith”, “234 Main St”);
document.write(bobSmith.info() + “
“);
document.write(“Bob is a person : ” + (bobSmith instanceof Person) + “
“);
function changeName(person){
person.name = “Sue Smith”;
}
changeName(bobSmith);
document.write(“Bob became ” + bobSmith.name + “
“);
var person1 = new Person(“Paul”, “123 Main”);
var person2 = new Person(“Paul”, “123 Main”);

document.write(“Are they equal ” + (person1 == person2) + “
“);
