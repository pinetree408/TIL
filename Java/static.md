static means that the variable or method marked as such is available at the class level.
In other words, you don't need to create an instance of the class to access it.

```
public class Foo {
    public static void doStuff(){
        // does stuff
    }
}

```

Instead of creating an instance of Foo and then calling doStuff like this:

```
Foo f = new Foo();
f.doStuff();
```

You just call the method directly against the class, like so:

```
Foo.doStuff();
```
