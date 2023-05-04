Download Link: https://assignmentchef.com/product/solved-cs4375-homework-1-data-exploration-with-r-and-c
<br>
<h1>Part 1: Rstudio Data Exploration</h1>

For each step below, place your code in the grey {r} boxes, and place comments and answers to questions in the white space above the code which you will label with a step number comment like this: <strong># Step 1</strong>, which makes ‘Step 1’ into a large heading.

<ol>

 <li>Create a new .Rmd file. Load library MASS. The first time you use a library you will have to install it, but do that at the console, <u>not in your R code</u>. After you load the library, look at the Environment pane in the upper right corner of RStudio. Notice that Boston is listed as &lt;Promise&gt;. When you load the package, R will be aware of the datasets in the package but won’t waste memory loading them until you use the data. We want to use the Boston data set, so load that into memory with data(Boston).  Use the str() function to get an overview of the data. Type ?Boston <em>at the console</em> (not in your code) and you will see a description of the data set in the lower right hand corner of Rstudio. Write a brief 2-3 sentence description of the data set in the white text portion of your answer for #1.</li>

 <li>Use R commands to:

  <ol>

   <li>display the first few rows &gt;&gt;</li>

   <li>display the last 2 rows &gt;&gt;</li>

   <li>display row 5 &gt;&gt;</li>

   <li>display the first few rows of column 1 by combining head() and indexing &gt;&gt;</li>

   <li>display the variable names &gt;&gt;</li>

  </ol></li>

 <li>Use R statistical functions to find the mean, median, range of the crime column.</li>

 <li>Create a histogram of the crime column, with an appropriate main heading. What does the histogram tell you about this variable?</li>

 <li>Use the cor() function to see if there is a correlation between crime and the median house value. Comment on what this value might mean. How useful might the crime column be for predicting median value?</li>

 <li>Create a plot showing the median value on the y axis and number of rooms on the x axis. Create appropriate main, x and y labels, change the point color and style. Reference:</li>

</ol>

<u>http://www.statmethods.net/advgraphs/parameters.html</u> Use the cor() function to quantify

the correlation between these two variables. Write a sentence summarizing what the graph and correlation tell you about these 2 variables.

<ol start="7">

 <li>Use R functions to determine if variable chas is a factor. Plot median value on the y axis and chas on the x axis. Make chas a factor and plot again. Comment on the difference in meaning of the two graphs. Look back the description of the Boston data set you got with the ?Boston command to interpret the meaning of 0 and 1.</li>

 <li>Explore the rad variable. What kind of variable is rad? What information do you get about this variable with the summary() function? Does the unique() function give you additional information? Use the sum() function to determine how many neighborhoods have rad equal to 24. Use R code to determine what percentage this is of the neighborhoods.</li>

 <li>Create a new variable called “far” using the ifelse() function that is TRUE if rad is 24 and false otherwise. Make the variable a factor. Plot far and medv. What does the graph tell you?</li>

 <li>Create a summary of Boston just for columns 1, 6, 13 and 14 (crim, rm, lstat, medv). Use the which.max() function to find the neighborhood with the highest median value. Display that row from the data set, but only columns 1, 6, 13 and 14. Write a few sentences comparing this neighborhood and the city as a whole in terms of: crime, number of rooms, lower economic percent, median value.</li>

</ol>

<h1>Part 2:  C++ Program</h1>

In this course we will get some experience writing machine learning algorithms from scratch in C++, and comparing performance to R. Part 2 of Homework 1 is designed to lay the foundation for writing custom machine learning algorithms in C++.

To complete Part 2, first you will need to export the Boston data frame from within R with a function like write.csv(), and then copy the csv file to your C++ folder.  You can just export the rm and medv columns to make reading the file easier in C++.

<ol>

 <li>Read the csv file (now reduced to 2 columns) into 2 vectors of the appropriate type.</li>

 <li>Write the following functions:

  <ol>

   <li>a function to find the sum of a numeric vector</li>

   <li>a function to find the mean of a numeric vector</li>

   <li>a function to find the median of a numeric vector.</li>

   <li>a function to find the range of a numeric vector</li>

   <li>a function to compute covariance between rm and medv (see formula below)</li>

   <li>a function to compute correlation between rm and medv (see formula below); Hint:</li>

  </ol></li>

</ol>

sigma of a vector can be calculated as the square root of variance(v, v)

<ol start="3">

 <li>Call the functions described in a-d for rm and for medv. Call the covariance and correlation functions. Print results for each function.</li>

</ol>




<table width="542">

 <tbody>

  <tr>

   <td width="274">Element</td>

   <td width="268">Points</td>

  </tr>

  <tr>

   <td width="274">Program run correctly (R and C++)</td>

   <td width="268">20 points: 10 pts each program (R, C++)</td>

  </tr>

  <tr>

   <td width="274">Appropriate comments and white space</td>

   <td width="268">20 points: 10 pts each program (R, C++)</td>

  </tr>

  <tr>

   <td width="274">Part 1: Steps 1-10</td>

   <td width="268">30 points</td>

  </tr>

  <tr>

   <td width="274">Part 2: Steps 1-3</td>

   <td width="268">30 points</td>

  </tr>

 </tbody>

</table>




Formulas:























