# -----------Abstract class---------------------------

# Can only be inherited, not instacied
# Poses abastract methods(is not implemented within the class but by its children)


# -----------Polimorphism -----------------------------
 
 # Is a ability a concrete class in runtime use the methods of its parent classes, however those methods
  # must have the same name/description as the parent class
  # Ex:

   public class Animal {

    void eat("I'm starving");

   }
  

  public Catte extends Animal {

    void eat() {
        println("I love hay");
    }

    void makeSound() {
        println("Mooh");
    }

    Public class Exec {

        public static void Main() {

            Animal cattle = new Catte();
            cattle.eat(); //Must print  "I love hay"
        }
    }
    

  }

# -------------------------------------