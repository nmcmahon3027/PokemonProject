# PokemonProject

//IDEAS:
//can create a super class: Pokemon
//reference them through polymorphism (look @ Notes part38)
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
    
    
    _.--""`-..
            ,'          `.
          ,'          __  `.
         /|          " __   \
        , |           / |.   .
        |,'          !_.'|   |
      ,'             '   |   |
     /              |`--'|   |
    |                `---'   |
     .   ,                   |                       ,".
      ._     '           _'  |                    , ' \ `
  `.. `.`-...___,...---""    |       __,.        ,`"   L,|
  |, `- .`._        _,-,.'   .  __.-'-. /        .   ,    \
-:..     `. `-..--_.,.<       `"      / `.        `-/ |   .
  `,         """"'     `.              ,'         |   |  ',,
    `.      '            '            /          '    |'. |/
      `.   |              \       _,-'           |       ''
        `._'               \   '"\                .      |
           |                '     \                `._  ,'
           |                 '     \                 .'|
           |                 .      \                | |
           |                 |       L              ,' |
           `                 |       |             /   '
            \                |       |           ,'   /
          ,' \               |  _.._ ,-..___,..-'    ,'
         /     .             .      `!             ,j'
        /       `.          /        .           .'/
       .          `.       /         |        _.'.'
        `.          7`'---'          |------"'_.'
       _,.`,_     _'                ,''-----"'
   _,-_    '       `.     .'      ,\
   -" /`.         _,'     | _  _  _.|
    ""--'---"""""'        `' '! |! /
                            `" " -'

    }

CLASS: Squirtle.java 

    public class Squirtle extends Pokemon {

    //if I were to do this below it would OVERWRIDEs Super class method

    void eat() { //MUST have the same name (eat) to take presidence
    System.out.println("A Squirtle has eaten");  //OUTPUT: A Squirtle has Eaten
                                          //        Eat (x3)
					  
	
	
	  _,........__
            ,-'            "`-.
          ,'                   `-.
        ,'                        \
      ,'                           .
      .'\               ,"".       `
     ._.'|             / |  `       \
     |   |            `-.'  ||       `.
     |   |            '-._,'||       | \
     .`.,'             `..,'.'       , |`-.
     l                       .'`.  _/  |   `.
     `-.._'-   ,          _ _'   -" \  .     `
`."""""'-.`-...,---------','         `. `....__.
.'        `"-..___      __,'\          \  \     \
\_ .          |   `""""'    `.           . \     \
  `.          |              `.          |  .     L
    `.        |`--...________.'.        j   |     |
      `._    .'      |          `.     .|   ,     |
         `--,\       .            `7""' |  ,      |
            ` `      `            /     |  |      |    _,-'"""`-.
             \ `.     .          /      |  '      |  ,'          `.
              \  v.__  .        '       .   \    /| /              \
               \/    `""\"""""""`.       \   \  /.''                |
                `        .        `._ ___,j.  `/ .-       ,---.     |
                ,`-.      \         ."     `.  |/        j     `    |
               /    `.     \       /         \ /         |     /    j
              |       `-.   7-.._ .          |"          '         /
              |          `./_    `|          |            .     _,'
              `.           / `----|          |-............`---'
                \          \      |          |
               ,'           )     `.         |
                7____,,..--'      /          |
                                  `---.__,--.'


    }
    }

CLASS: Pikachu.java

    public class Pikachu extends Pokemon {
    
    
    
         ,-.
                                          _.|  '
                                        .'  | /
                                      ,'    |'
                                     /      /
                       _..----""---.'      /
 _.....---------...,-""                  ,'
 `-._  \                                /
     `-.+_            __           ,--. .
          `-.._     .:  ).        (`--"| \
               7    | `" |         `...'  \
               |     `--'     '+"        ,". ,""-
               |   _...        .____     | |/    '
          _.   |  .    `.  '--"   /      `./     j
         \' `-.|  '     |   `.   /        /     /
         '     `-. `---"      `-"        /     /
          \       `.                  _,'     /
           \        `                        .
            \                                j
             \                              /
              `.                           .
                +                          \
                |                           L
                |                           |
                |  _ /,                     |
                | | L)'..                   |
                | .    | `                  |
                '  \'   L                   '
                 \  \   |                  j
                  `. `__'                 /
                _,.--.---........__      /
               ---.,'---`         |   -j"
                .-'  '....__      L    |
              ""--..    _,-'       \ l||
                  ,-'  .....------. `||'
               _,'                /
             ,'                  /
            '---------+-        /
                     /         /
                   .'         /
                 .'          /
               ,'           /
             _'....----""""" 


    }

(Super)CLASS: Pokemon

    public class Pokemon {

    void eat() {
    System.out.println("Eat");

    }
    }



//Example of title


	private static String[] pokeTitle = { 
		"                               .::.                           ",
		"                              .;:**'                          ",
		"                              `                               ",
		"  .:XHHHHk.              db.   .;;.     dH  MX                ",
		"oMMMMMMMMMMM       ~MM  dMMP :MMMMMR   MMM  MR      ~MRMN     ",
		"QMMMMMb  'MMX       MMMMMMP !MX' :M~   MMM MMM  .oo. XMMM 'MMM",
		"  `MMMM.  )M> :X!Hk. MMMM   XMM.o'  .  MMMMMMM X?XMMM MMM>!MMP",
		"   'MMMb.dM! XM M'?M MMMMMX.`MMMMMMMM~ MM MMM XM `' MX MMXXMM ",
		"    ~MMMMM~ XMM. .XM XM`'MMMb.~*?**~ .MMX M t MMbooMM XMMMMMP ",
		"     ?MMM>  YMMMMMM! MM   `?MMRb.    `MM   !L'MMMMM XM IMMM   ",
		"      MMMX   'MMMM'  MM       ~%:           !Mh.''' dMI IMMP  ",
		"      'MMM.                                             IMX   ",
		"       ~M!M                                             IM    " 
	};
