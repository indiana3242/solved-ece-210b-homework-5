Download Link: https://assignmentchef.com/product/solved-ece-210b-homework-5
<br>



In this homework, we will go through a few advanced data structures in MATLAB, such as cell arrays, classes, chars, as well as dataset importing in MATLAB. You will be importing in the fisheriris dataset and encapsulating it in classes. After obtaining all the data, you will be required to write some methods for the class you just created. Also note that some operations will require you to do some research, but not too much!

<ol>

 <li>Load in the <em>fisheriris </em>dataset with the command <em>load fisheriris</em>. You should obtain a 150×4 matrix called meas, as well as a 150×1 cell array called species in your workspace. This is a very popular dataset, and you can quickly google fisheriris to see what the columns of meas represent.</li>

</ol>

<ul>

 <li>Create a class called <em>Flower </em>in its own .m file. In your <em>Flower </em>class, you should have the following properties – petalWidth (double), petalLength(double), sepalWidth (double), sepalLength (double) and species (char). The ith species corresponds to the ith row of information in meas. Note that you do not need to specify the data type of the properties when you are declaring a class the following properties are just here to impress on you what type of properties you would be expecting.</li>

 <li>Create a constructor for your class. It should take in 4 doubles and a char array corresponding, in order, to the five properties of your class.</li>

 <li>Now, import the entries from meas and species into MATLAB and store them in a 150×1 cell array of <em>Flower </em> You can either use a for loop to import the entries, or use a more elegant way to make all entries in one line (this would require some research on object formation in MATLAB). Either way is ok. However, note that the name of the species are stored as cell arrays; make sure to <strong>extract </strong>from the cell as a char and <strong>remove trailing white spaces </strong>before storing them in the <em>Flower </em>instances. There is a single function that will do this, which you should be able to find with a quick google search.</li>

 <li>Create a method called <em>getSWidth </em>for the <em>Flower </em>class, which will return the sepal length of the object. Use this on the 30th Flower in your cell array, and check (using ==) that this is the correct value by looking that the corresponding entry in meas.</li>

 <li>Create another method called <em>report </em>for the <em>Flower </em>object, which will print out a statement on the command window and report the details about the <em>Flower </em> This function does not need to return anything. It should print out a statement of the following form if the flower is 5.1 cm in sepal length, 3.5 cm in sepal width, 1.4 cm in petal length and 0.2 cm in petalWidth, and the species is setosa, for example: “The length and width of its sepal are 5.1 cm and 3.5cm respectively, while the length and width of its petal are 1.4cm and 0.2cm respectively. It belongs to the setosa species.”</li>

</ul>

1