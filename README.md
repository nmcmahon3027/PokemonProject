# PokemonProject

//IDEAS:
//can create a super class: Pokemon
//refernce them through polymorphism (look @ Notes part38)
//Polymorphic Arrays



App.java    Charmander.java     Squirtle.java  Pikachu.java     Pokemon.java

    public class App {

    public static void main(String[] args) {

    Pokemon allPokemon[] = new Pokemon[4];//# of OBJECTS(0,1,2,3)  //specifying SUPER CLASS
                                    //Declaring Array type of Pokemon (super class type)
    allPokemon[0] = new Charmander();
    allPokemon[1] = new Squirtle();       //can put any subclass of Pokemon inside array
    allPokemon[2] = new Pikachu();
    allPokemon[3] = new Weedle(); //adding to array

    for (int i = 0; i < allPokemon.length; i++); //loop through the array

    allPokemon [i].eat(); //can call any of the SUPER CLASS MEHTODS
                          //eat() method is just a place holder currently for testing

    }

    }
    }

(Inheritence) Classes (Other Pokemon)

CLASS: Charmander.java

    public class Charmander extends Pokemon {

    }

CLASS: Squirtle.java 

    public class Squirtle extends Pokemon {

    //if I were to do this below it would OVERWRIDEs Super class method

    void eat() { //MUST have the same name (eat) to take presidence
    System.out.println("A Squirtle has eaten");  //OUTPUT: A Squirtle has Eaten
                                          //        Eat (x3)

    }
    }

CLASS: Pikachu.java

    public class Pikachu extends Pokemon {

    }

(Super)CLASS: Pokemon

    public class Pokemon {

    void eat() {
    System.out.println("Eat");

    }
    }
