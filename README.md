Download Link: https://assignmentchef.com/product/solved-stat542-assignment-1
<br>
This assignment is related to the simulation study described in Section 2.3.1 (the so-called Scenario 2) of “Elements of Statistical Learning” (ESL).

<strong>Scenario 2</strong>: the two-dimensional data <em>X </em>∈ <strong>R</strong><sup>2 </sup>in each class is generated from a mixture of 10 different bivariate Gaussian distributions with uncorrelated components and different means, i.e.,

<em>,</em>

where <em>k </em>= 0<em>,</em>1, <em>l </em>= 1 : 10, <em>P</em>(<em>Y </em>= <em>k</em>) = 1<em>/</em>2, and <em>P</em>(<em>Z </em>= 1) = 1<em>/</em>10<em>. </em>In other words, given <em>Y </em>= <em>k</em>, <em>X </em>follows a mixture distribution with density function

<em>.</em>

You can choose your own values for <em>s </em>and the twenty 2-dim vectors <strong>m</strong><em><sub>kl</sub></em>, or you can generate them from some distribution.

Repeat the following simulation 20 times. In each simulation, following the data generating process,

<ol>

 <li>generate a training sample of size 200 and a test sample of size 10,000, and</li>

 <li>calculate the <strong>training </strong>and <strong>test </strong>errors (the averaged 0/1 error<sup>1 </sup>) for the following four procedures:</li>

</ol>

<ul>

 <li>Linear regression with cut-off value 0<em>.</em>5,</li>

 <li>quadratic regression with cut-off value 0<em>.</em>5,</li>

 <li><em>k</em>NN classification with <em>k </em>chosen by 10-fold cross-validation, and</li>

 <li>the Bayes rule (assume your know the values of <strong>m</strong><em><sub>kl</sub></em>’s and <em>s</em>).</li>

</ul>

Summarize your results on training errors and test errors graphically, e.g., using boxplot or stripchart. Also report the mean and standard error for the selected <em>k </em>values.

R packages you are allowed to use are class (for <em>k</em>NN) and ggplot2 (for graphs).

<sup>1</sup>For each sample, the incurred error is 1 if there is a mistake, and 0 otherwise.

<strong>What you need to submit?</strong>

A PDF file and an R Markdown file that produces the PDF file.

<ul>

 <li>Name your files starting with</li>

</ul>

Assignment 1 xxxx netID where “xxxx” is the last 4-dig of your University ID.

For example, the submission for Max Y. Chen with UID 672757127 and netID mychen12 would be named as

Assignment 1 7127 mychen12 MaxChen.Rmd/.pdf

You can add whatever characters after your netID.

<ul>

 <li>Set the seed at the beginning of your code to be the last 4-dig of your University ID. So once we run your code, we can get the same result.</li>

</ul>