# Java Setup

## Make sure future java classwork is organized
```
cd ~
mkdir java
cd java
mkdir java-apcsa
cd java-apcsa
mkdir u0-other u1-intro u2-conditionals-loops u3-strings-1d-arrays u4-methods u5-user-classes u6-advanced-classes u7-algorithms u8-2d-arrays u9-ap-review
```

## Make a template file
* `touch template.java`
* Open it, then paste the following code:
```java
import java.util.Scanner;
import java.lang.Math;

class Main {
    public static void main(String[] args) {

        Scanner scan = new Scanner(System.in);

        System.out.println("Hello World");

    }
}
```

## Hello World
```
cd u0
mkdir HelloWorld
cd HelloWorld
touch Main.java
```
* Open `Main.java` and paste in the same code from your template
* `javac Main.java`
* `java Main`
* You should see `Hello World` in your terminal

* As a general rule of thumb, use this same format when making new programs (`cd` into the correct directory, make a folder with the appropriate name, `cd` into it, then name your file `Main.java` which will then get compiled to `Main.class`)
  * As a shortcut, you can copy with the `cp source destination` command. I.e. once you make your `HelloWorld` directory and `cd` into it, you could do `cp ~/java/java-apcsa/template.java ./Main.java`

## Java compile and run
#### Setting this up allows you to compile and run in the same command
`nano ~/.bash_profile`  
Paste the following:  
`jcar() { javac $1.java && java $1 ; }`  
Do <kbd>control</kbd>+<kbd>X</kbd> to quit, <kbd>Y</kbd> to save, then press <kbd>ENTER</kbd>
#### To use, type `jcar Program` (using your own Java program file, but with no .java)
* Try this out by adding `!` to your **Hello World** program so that it outputs `Hello World!`
* Run the shortcut by doing `jcar Main`
