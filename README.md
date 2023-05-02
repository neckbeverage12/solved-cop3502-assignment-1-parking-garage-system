Download Link: https://assignmentchef.com/product/solved-cop3502-assignment-1-parking-garage-system
<br>
For this assignment, you will use Java and Eclipse. In this assignment we will create a system for parking garages at UCF. We will use the concept of abstract class, interface, string and file operations. The top of your ALL source files must contain the following course header (with correct assignment number) identifying you as an author:

<strong>Compliance with Rules:</strong> UCF Golden rules apply towards this assignment and submission. Programming assignment rules mentioned in syllabus, are also applied in this submission.

<strong>Eclipse Implementation: </strong>

<ol>

 <li>Create a Java project in Eclipse called “ParkingGarageSystem”.</li>

 <li>You will need to create 4 java classes in the “src” subfolder of the package.</li>

 <li>The ABSTRACT class would be Garage (Eclipse will put this class in the file “Garage.java”). This is a base class for garages.</li>

 <li>Next there would be one interface, ParkingSpot (Eclipse will put this class in the file “ParkingSpot.java”).</li>

 <li>The third class would be GarageC (Eclipse will put this class in the file “GarageC.java”). This class will inherit properties from Garage class and implement ParkingSpot interface.</li>

</ol>




<ol start="3">

 <li>Add the course header with your name at the top of the file.</li>

 <li>Write your Java codes.</li>

 <li>Save your Java codes.</li>

 <li>Run your Java codes.</li>

 <li>Submit only the four mentioned java source files on webcourses (Please DO NOT submit the compressed project or JAR file).

  <ol>

   <li>java</li>

   <li>java</li>

   <li>java</li>

   <li>java</li>

  </ol></li>

</ol>




<strong>Provided Resources: </strong>

<strong> </strong>

A text file “cars.txt”. You can use this text file to test your code, however we will be grading your submission with a DIFFERENT text file. There are tabs(“t”) between the words and numbers. The test case text file will be of same format of the given cars.txt file, only with different car names, width, and length.




<strong>The Problem: </strong>




In this problem we will try to learn and implement abstract class and interface. We will also learn to do the String and File operations. We will create 3 classes to maintain the parking system of UCF. For the sake of simplicity, we will consider only three types of cars (irrespective of make and model): Small, Medium, Large. Your job is to read the text file containing all the car information at a time, and determine:

<ul>

 <li>How occupied the garage is,</li>

 <li>How many different types of cars are present in the garage, (iii) If the garage is still OPEN or FULL.</li>

</ul>

From implementational point of view, here are certain points which could be helpful:

<ol>

 <li>The base class (which is also abstract) Garage has the following features:

  <ol>

   <li>A private variable to take garage name</li>

   <li>A constructor for setting the garage name</li>

   <li>A getter method for garage name</li>

   <li>An abstract method to calculate the total occupied area for a garage. <strong>Hint- the input argument is an Arraylist containing the areas of all the cars. </strong></li>

  </ol></li>

</ol>




<ol start="2">

 <li>The ParkingSpot interface has the following features. Note that the methods will not be implemented within the interface:

  <ol>

   <li>A method specification which takes the width and length of a car and returns the type of the parking (Small/Medium/Large), needed for the car. The length range for those three types of cars are: Small (&lt;=15 feet), Medium (&gt; 15 but &lt;=17), and Large (&gt; 17).</li>

   <li>A method which will return the area of a parking spot, taking width and length of the car as arguments. Take the width and length as double.</li>

  </ol></li>

</ol>




<ol start="3">

 <li>The class GarageC will inherit all the properties from Garage and implement the all properties from ParkingSpot. It has some extra features:

  <ol>

   <li>A private variable for number of floors. Type: Integer.</li>

   <li>A private variable for each floor area. Type: Double.</li>

   <li>A <strong>PRIVATE </strong>constructor that will initialize the instance variables of GarageC. It will take three arguments, garage name, number of floors, and each floor area.</li>

   <li>You have to implement Single tone design pattern. The whole system cannot have more than one GarageC object. So, create a factory method that utilize the singleton design pattern and prevent to have more than one object of GarageC.</li>

   <li>A getter method for number of floors variable.</li>

   <li>A getter method for each floor area variable.</li>

   <li>Properly implement the interface methods and abstract method.</li>

  </ol></li>

</ol>




<ol start="4">

 <li>Create a GarageTest class and it should contain the main method. In the main method, please take three input for GarageC: one for number of floors of Garage C (point 3.a), second for each floor area of Garage C (point 3.b), and lastly the filename, (for example “cars.txt” file). You should keep the file in appropriate directory so that your program can read it.

  <ol>

   <li>Please read the file using proper file operations.</li>

   <li>Perform the proper string operations and get width and length for each car.</li>

   <li>Determine parking spot’s type for each car.</li>

   <li>Determine parking spot area for each car.</li>

   <li>While adding the cars in the garage from the file, determine the total area occupied in Garage C after reading each car. Also, and print the information in the console like this (Car: truck1, parking type: Large, Area: 150, Total area occupied in Garage C: 150.66, Total vacant area in Garage C: 500)</li>

   <li>Whenever, the Garage C becomes full, print it in the console “Garage C is full” and write the list of the car type and their count into a text file called “out.txt” (example: small: 3, medium: 2). To taste this part of the code, you need to provide a relatively smaller number of floor and area for each floor, so that the garage becomes full with the input data from the file.</li>

  </ol></li>

</ol>




<strong>Sample Input/Output Format: </strong>

<strong> </strong>

Enter number of floor: 2

Enter area at each floor: 500

Enter input file name: cars.txt

Car: truck1, parking type: Large, Area: 150.66, Total area occupied in Garage C: 150, Total vacant area in Garage C: 850 //because 500*2 – 150 ….

…..

If at any point the total area occupied exceeds 1000, it should display full and write out.txt with the information as require din in 4.f above.

<strong> </strong>


