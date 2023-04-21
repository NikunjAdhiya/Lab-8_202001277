# <pre>                  IT314 - Software Engineering </pre>

#### Name       : Nikunj Adhiya
#### Student ID  : 202001277
#### Date       : 21-04-2023

----

## Objective:
    The goal of this lab is to learn how to use JUnit to write unit tests for Java programs.
   
----
1. Creating eclipse project named 'Lab8' and a package named 'myPackage' inside src folder in it.
![1](https://user-images.githubusercontent.com/86603004/233598654-aec48333-8028-401c-8a0d-add0a6684a49.png)



2. Creating a class for a Boa with the given code snippet in the lab manual.
```
public class Boa {
	private String name;
	private int length; // the length of the boa, in feet
	private String favoriteFood;
	
	public Boa (String name, int length, String favoriteFood){
		this.name = name;
		this.length = length;
		this.favoriteFood = favoriteFood;
	}
	
	//returns true if this Boa constructor is healthy
	public boolean isHealthy(){
		return this.favoriteFood.equals("granola bars");
	}
	
	//returns true if the length of this Boa constructor is
	//less than the given cage length
	public boolean fitsInCage(int cageLength){
		return this.length < cageLength;
	}
}	
```
![2](https://user-images.githubusercontent.com/86603004/233598747-6139b632-63db-4f2d-a544-5c7a6418276a.png)


3.Then I created a JUnit test file for the Boa Class with name <b>BoaTest</b>
![3](https://user-images.githubusercontent.com/86603004/233598793-47d6da00-092a-40e8-9ea4-9aaf01619070.png)


4.Then I modified the setUp method to initialize the variables.

5.Then I also implemented tests for the given two functions <b>testIsHealthy()</b> and <b>testFitsInCage()</b>.
![4](https://user-images.githubusercontent.com/86603004/233598875-853744ad-c6a0-4fa6-8617-aca4e81eac17.png)



For testing thee fitsInCage() function, there is no need to write tests for both jen and ken objects as the function is same for both and the output of test cases depends only whether the given lenght is greater than,less than or equal to actual length of object.The behaviour will be similar in both cases.

6.Then I ran the Junit test file and all the tests are passed.There are no red bars in the output.

![5](https://user-images.githubusercontent.com/86603004/233598942-bbff144c-b41c-4204-b246-bd752a86d921.png)


It can be seen that 2 out of 2 test cases have been passed. 

7.Then I added a new method to the Boa class with name <b>lenghtInInches()</b> to get the length in inches.

![6](https://user-images.githubusercontent.com/86603004/233599040-458ad6e6-89fb-40ce-9a1a-30be403c166f.png)


As the length of the Boa is given in feet, to convert it into inches, I had multiplied length with 12 and returned the value.


8.Then I wrote another test case for this new method and ran the 3 test cases together. 

![7](https://user-images.githubusercontent.com/86603004/233599067-37cc0969-ef10-4a16-bbe1-6bcd52bdfe28.png)


Thus, test cases have been written for the given Boa class and all the three methods have been tested with required Junit test cases.
