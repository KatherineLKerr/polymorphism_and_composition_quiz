# Polymorphism & Composition Answers

## polymorphism
1. Polymorphism is made of "poly" which means "many", and "morph" which means "change".

2. It means that an object can take on different forms. It could be treated as a class it has inherited from or be treated as a type of interface it implements.

```java
public class InstrumentList {

    ArrayList<Instrument> instruments;
    private Guitar guitar;
    private Drums drums;

    public InstrumentList() {
        this.instruments = new ArrayList();
        this.guitar = new Guitar(); //Guitar class extends Instrument class
        this.drums = new Drums(); //Drums class extends Instrument class
    }

    public void addPlant(Plant plant) {
        this.instruments.add(guitar);
        this.instruments.add(drums);
    }

}
```

3. We can use inheritance or interfaces to implement polymorphism in java. If using inheritance it takes the form of the parent class. If using interfaces it takes the form of the interface, and any methods that aren't on the interface cant be accessed.

4. An object can take on as many forms as it has classes it inherits from or interfaces it implements when using polymorphism. Only one at a time though.

5. When you need to make an array list of different objects. If they all implement the same interface or inherit from the same class, you can use polymorphism to treat them as the same type. This will allow them to be added to the same array list even thought they are different classes.

## composition
6. Composition means when an object has a "has a" relationship with another object.

7. You would use composition when you need to use one or more objects inside another object.

```java
public Phone(Screen screen, Buttons buttons, Speaker speaker) {
  this.screen = screen;
  this.buttons = buttons;
  this.speaker = speaker;
}
```

8. Advantages of composition are that the object can use any methods/behaviours from objects it is composed of. An object can be composed of many others rather than inheritance where it can only inherit from one.  

9. When an object is destroyed, any objects it is composed of are also destroyed.
