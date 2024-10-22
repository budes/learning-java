Class -> Object

Basically our way of coding something from outside the scope of the language.
Let's say we want to code in something like a car. The car object has it's own properties, like model, year, color, engine size, number of seats, has it been checked up recently, mileage, things that matter for a car. So if we define a car in coding, it would be something like:

```
car {
 model: string;
 year: int;
 color: string;
 engineSize: double;
 numberOfSeats: int;
 checkedUp: boolean;
 mileage: int or double;x
}
```

So if we define the object "car" when we design something to sell cars, for example, we will just need to define those things and then publish the model, with the pricing of the listing, so, if the listing was also an object:

```
listing {
  objectToSell: class;
  pricing: double; 

  sell(){ } -> Sell item and update listing if needed
}
```

It makes things easier to structure if we can make objects out of them that interacts directly with our code. Now it's easier to understand that is a car, that is a listing, and everything we are doing right now, also, it standardizes the process too, making it easier to scale.

----
## The actual coding

### How to define a class
Using the previous example as an example, we can start the `car` object by doing:
```
public class Car { // It is a *public* class so we can access it externally
	// Our code would go here
}
```

### How to make it build itself
After we make our class `Car`, we need to make it declare our needed variables, and put them in the right place, so we can work with it better. (for our example, i will just put model, color and it has been checked up)

```
public class Car {
	// All of these variables are *public* so we can access it externally
	public String model;
	public String color;
	public boolean checkedUp;
	
	public Car(String modelOfTheVehicle, String colorOfTheVehicle, boolean hasBeenCheckedUp) {
		model = modelOfTheVehicle;
		color = colorOfTheVehicle;
		checkedUp = hasBeenCheckedUp;
	}
}
```

Our method `Car` would be our constructor. The part that will define where each argument will go, and also, the attributes of our class.
That part will be "activated" after we put `new OurObject(arguments)` -> The instantiation of our object.

It will automatically attribute everything to it's spots correctly, so the user can not only interact with it, but the own class can use it too.

We can define different constructors for different arguments too.
Let's say we want to define a single class for both gas and electric fueled cars. For that we can use two constructors.

```
public Car(boolean IsEletric, String model, int year, int mpg) {}
public Car(String model, int year, int mpg) {}
```

So we won't need an if statement or anything like that, just two constructors, if it detects a boolean in the beginning, it knows to use the first constructor.