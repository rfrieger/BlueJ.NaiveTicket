# NaiveTicket

The second Objects lab, from the BlueJ book's second chapter.

Look for the [Chapter 2 file](./doc/BlueJ-objects-first-ch2.pdf) you need in the [doc](./doc) folder.
There is 35 pages of reading and exercises in the chapter.

Work through all these exercises. You edit this file with your answers for these exercises.

### Exercise 2.1
* Create a TicketMachine object on the object bench.
* Upon viewing its methods, `getBalance`, `getPrice`, `insertMoney`, `printTicket`.
* Use `getPrice` method to view the value of the price of the tickets that was set when this object was created.
* Use `insertMoney` method to simulate inserting an amount of money into the machine.
* Use `getBalance` to check that the machine has a record of the amount inserted.
	* You can insert several separate amounts of money into the machine, just like you might insert multiple coins or notes into a real machine. Try inserting the exact amount required for a ticket. As this is a simple machine, a ticket will not be issued automatically, so once you have inserted enough money, call the `printTicket` method. A facsimile ticket should be printed in the BlueJ terminal window.

### Exercise 2.2
* What value is returned if you check the machine’s balance after it has printed a ticket?
	0

### Exercise 2.3
* Experiment with inserting different amounts of money before printing tickets.
	* Do you notice anything strange about the machine’s behavior?
		It will still print a ticket even if the amount for ticket is not inserted.
	* What happens if you insert too much money into the machine – do you receive any 
	refund?
		The balance is reduced to 0 and no refund.
	* What happens if you do not insert enough and then try to print a ticket?
		It will still print.

### Exercise 2.4
* Try to obtain a good understanding of a ticket machine’s behavior by interacting with it on the object bench before we start looking at how the `TicketMachine` class is implemented in the next section.

### Exercise 2.5
* Create another ticket machine for tickets of a different price.
	* Buy a ticket from that machine.
	* Does the printed ticket look different?
		No, it is the same.

### Exercise 2.6
* Write out what you think the outer wrappers of the `Student` and `LabClass` classes might look like – do not worry about the inner part.
	
	public class Student() {}
	public class LabClass() {}


### Exercise 2.7
Does it matter whether we write<br>
`public class TicketMachine`<br>
or<br>
`class public TicketMachine`<br>
in the outer wrapper of a class?

yes

* Edit the source of the `TicketMachine` class to make the change and then close the editor window.
	* Do you notice a change in the class diagram?
	* What error message do you get when you now press the compile button?
	* Do you think this message clearly explains what is wrong?
the class box get red X's and puts out the error '<idenifier> expected'. It is not clear at all.
### Exercise 2.8
* Check whether or not it is possible to leave out the word `public` from the outer wrapper of the `TicketMachine` class.

	It is possible.

### Exercise 2.9
* From your earlier experimentation with the ticket machine objects within BlueJ you can probably remember the names of some of the methods – `printTicket`, for instance.
	* Look at the class definition in Code 2.1 and use this knowledge, along with the additional information about ordering we have given you, to try to make a list of the names of the fields, constructors, and methods in the `TicketMachine` class.
	* Hint: There is only one constructor in the class.
	fields - price, balance, total
	methods - getPrice(), getbalance(), insertMoney(), printTicket()
	constructor - TicketMachine(int ticketCost)

### Exercise 2.10
* Do you notice any features of the constructor that make it significantly different from the other methods of the class? it takes arguments and the first letter is capitalized.

### Exercise 2.11
* What do you think is the type of each of the following fields?

```java
private int count; int
private Student representative; Student
private Server host; Server
```

### Exercise 2.12
* What are the names of the following fields?

```java
private boolean alive; alive
private Person tutor; tutor
private Game game;	game
```
### Exercise 2.13

In the following field declaration from the TicketMachine class<br>

```java
private int price;
```
does it matter which order the three words appear in?
* Edit the `TicketMachine` class to try different orderings. After each change, close the editor.
	* Does the appearance of the class diagram after each change give you a clue as to whether or not other orderings are
possible? it does and they are not.
	* Check by pressing the compile button to see if there is an error message.
	* Make sure that you reinstantiate the original version after your experiments!

### Exercise 2.14
* Is it always necessary to have a semicolon at the end of a field declaration? yes
* Once again, experiment via the editor.
* The rule you will learn here is an important one, so be sure to remember it.


### Exercise 2.15
* Write in full the declaration for a field of type `int` whose name is `status`.
 int status;

### Exercise 2.16
* To what class does the following constructor belong?
```
public Student(String name)
	Student
```

### Exercise 2.17
* How many parameters does the following constructor have and what are their types?
```
public Book(String title, double price)
	2 String and double
```

### Exercise 2.18
* Can you guess what types some of the `Book` class’s fields might be? String , Int
* Can you assume anything about the names of its fields?
	title, author,chapter length  

### Exercise 2.19 name = this.petsName;
### Exercise 2.20 price is typed twice.
### Exercise 2.21 nothing besides the names;
### Exercise 2.22 How much money has been inserted;
### Exercise 2.23 No because they both return int;
### Exercise 2.24 public int getTotal() { 
	return total;
}
### Exercise 2.25 missing return statment;
### Exercise 2.26 void return type;
### Exercise 2.27 printTicket doestn retrun anything hence its return value is void;	
### Exercise 2.29 the Name is not capitilezd;
### Exercise 2.30 see BlueJ.NaiveTicket 
### Exercise 2.31 score += points;
### Exercise 2.32 price -= amount;	
### Exercise 2.33 see BlueJ.NaiveTicket 
### Exercise 2.34 see BlueJ.NaiveTicket 
### Exercise 2.35 no because they are seperate intances of the class ticketMachine;
### Exercise 2.36 it would print the whole string without replacing price with the price inputed;
### Exercise 2.37 same as before would just print a String.
### Exercise 2.38 Because the var is within the "" it will be seen as just a string and not a var.
### Exercise 2.39 does not ask for parameters when object is created.
### Exercise 2.40 It does not need any parameters and it is a mutator;
### Exercise 2.41 Yes it is a mutator.
### Exercise 2.43 No the balance will only change is a positive number is put in as a prameter;
### Exercise 2.44 The behavior wouldn't change much other than not printing an error if 0 was entered;
### Exercise 2.45 We used it for the isVisible method, it was well suited because we only wanted to know if we want to display it or not, nothing else
### Exercise 2.46 It increases the total by the ticket cost and only reduces the balance by the ticket price rather than making it 0.
### Exercise 2.47 No, because the print ticket method checks that there is more or equal to the ticket price in the balance
### Exercise 2.49 int saving = price * discount;
### Exercise 2.50 int mean = total / count;
### Exercise 2.51/52 if (price > budget) {
	System.out.println("Too expensive");
	System.out.println(budget);

} else {
	System.out.println(Just right);
}

### Exercise 2.53 It differs because it will always refund 0 because its setting the balance to 0 everytime before returning balance; 
### Exercise 2.54 It wont complile because the the balance=0 statment can never be reached;
### Exercise 2.55 see BlueJ.NaiveTicket; 
### Exercise 2.56 It is both a accessor and a mutator;
### Exercise 2.57 see BlueJ.NaiveTicket; 




Work all Exercises from 2.19 to 2.58 that are **NOT** marked *Challenge exercise*.
READ upto and INCLUDING section 2.15 of this chapter.