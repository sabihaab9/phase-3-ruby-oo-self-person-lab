# OO Person Lab

## Learning Goals

- Gain proficiency instantiating a class
- Gain ability to discern when to implement `attr_accessor`, `attr_reader`, and
  `attr_writer`
- Gain ability to discern when to define your own `attr_reader` (getter) and
  `attr_writer` (setter) methods

  ## A Note on Notation

In the instructions below (and in other labs), you'll see this notation used to
represent instance methods and class methods:

1. *`ClassName#method_name`* --> is a **instance method** that can be called on the class.
2. *`ClassName.method_name`* ---> is a  **class method** that can be called on the class

For example, `Person#name` is an example of an instance method, that we can call
on an instance of a class:

```rb
class Person
  def name
    @name
  end
end
```

We can also define this particular instance method using a macro (which creates
the getter method for us):

```rb
class Person
  attr_reader :name

end
```

`Person.new` is an example of a class method (remember, to create a new instance
of the class, we call `ClassName.new`, which then calls the instance method
`ClassName#initialize`).
