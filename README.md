# Chapter-1-Lab-3

**OldMacDonald**

**Background:**

In this lab, we will use the well-known song 'Old MacDonald Had a Farm' to learn about Inheritance and Polymorphism. Old MacDonald had a farm and several types of animals. Every animal shared certain characteristics. They each had a type (such as cow, chick or pig) and each made a sound (moo, cluck or oink). An Interface defines those things required to be an animal on the farm.

**public interface** Animal{

**public** String getSound(); 

**public** String getType();

}

**Notes:** 

For those unfamiliar with it, a version of the _Old MacDonald_ song is found at [http://www.scoutsongs.com/lyrics/oldmacdonald.html](http://www.scoutsongs.com/lyrics/oldmacdonald.html). 

**Assignment:**

1. Once we know what it takes to be an Animal, we can define new classes for the cow, chick and pig that implement the Animal interface. Here is a Cow class meeting the minimum requirements to be an Animal.

**public class** Cow **implements** Animal{

   

**private** String myType;

**private** String mySound;

Cow(){

myType = “cow”;

mySound = “moo’;

}

**public** String getSound(){

**return** mySound; 

}

**public** String getType(){

**return** myType; 

}

} 

  

2.  Implement classes for the chick and the pig. Also complete the test program below to verify your work so far:

**public class** Main{

**public static void** main(String[] args){

Cow c = **new** Cow();

System.out.println( c.getType() + " goes " + c.getSound() );

// _< your code here >_

}

}  

[[1]](https://repl.it/teacher/assignments/2489991/edit#_ftnref1) This lab was adapted, with gratitude, from a lab developed by Roger Frank of Ponderosa HS, in Parker, CO. 
