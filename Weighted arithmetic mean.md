similar to an ordinary [[Arithmetic mean|arithmetic mean]] (the most common type of average), except that instead of each of the data points contributing equally to the final average, some data points contribute more than others.

if all the weights are equal, then the weighted mean is the same as the arithmetic mean. weighted means in general, behave the same as an arithmetic mean but have a few counterintuitive properties (such as in [[Simpson's paradox]])

## Examples

given two school classes–one with 20 students, and one with 30–and test grades from each class as follows:

Morning class = {62, 67, 71, 74, 76, 77, 78, 79, 79, 80, 80, 81, 81, 82, 83, 84, 86, 89, 93, 98}

Afternoon class = {81, 82, 83, 84, 85, 86, 87, 87, 88, 88, 89, 89, 89, 90, 90, 90, 90, 91, 91, 91, 92, 92, 93, 93, 94, 95, 96, 97, 98, 99}

the mean for the morning class is 80 and the mean for the afternoon class is 90. the unweighted mean of the two means is 85.

however this does not account for the difference in number of students in each class (20 versus 30); so the value of 85 does not reflect the average student grade (independent of which class they were in).

there are two ways to solve this problem, the first being simply adding up all the grades and dividing by the total number of students (obtaining the arithmetic mean)

$$
\overline{x}=\frac{4300}{50}=86
$$

or you can weigh the class means by the number of students in each class, therefore giving the larger class more "weight":

$$
\overline{x}=\frac{(20\times80)+(30\times90)}{20+30}=86
$$

