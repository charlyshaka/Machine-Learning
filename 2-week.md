## Linear Regression with Multiple Variables
---
1. Suppose m=4 students have taken some class, and the class had a midterm exam and a final exam. You have collected a dataset of their scores on the two exams, which is as follows:

| midterm exam | (midterm exam)^2 | final exam |
|--------------|------------------|------------|
| 89 | 7921 | 96 |
|72|5184|74|
|94|8836|87|
|69|4761|78|

You'd like to use polynomial regression to predict a student's final exam score from their midterm exam score. Concretely, suppose you want to fit a model of the form h_\theta(x) = \theta_0 + \theta_1 x_1 + \theta_2 x_2 , where x_1 is the midterm score and x_2 is (midterm score)^2 2 . Further, you plan to use both feature scaling (dividing by the "max-min", or range, of a feature) and mean normalization. What is the normalized feature x_1^{(3)} ? (Hint: midterm = 94, final = 87 is training example 3.) Please round off your answer to two decimal places and enter in the text box below.

Answer: The mean of x1 is 81 and the range is 94−69=25  So x<sub>1</sub><sup>(3)</sup> is 94−81/25=0.52.

---
2. You run gradient descent for 15 iterations with α=0.3 and compute J(θ) after each iteration. You find that the value of $$ J(θ) $$ decreases slowly and is still decreasing after $ 15 $ iterations. Based on this, which of the following conclusions seems most plausible?

Answer: Rather than use the current value of α, it'd be more promising to try a larger value of  (α=1.0).
---
3. Suppose you have m = 23 training examples with n = 5 features (excluding the additional all-ones feature for the intercept term, which you should add). The normal equation is \theta = (X^TX)^{-1}X^Tyθ=(X T X) −1 X T y. For the given values of mm and nn, what are the dimensions of \thetaθ, XX, and yy in this equation?

Answer:  is X 23×6, y 23×1, \thetaθ is 6×1
---
4. Suppose you have a dataset with m = 50 examples and n = 200000n=200000features for each example. You want to use multivariate linear regression to fit the parameters \thetaθ to our data. Should you prefer gradient descent or the normal equation?

Answer: Gradient descent, since (X^TX)^{-1} will be very slow to compute in the normal equation.
---
5.Which of the following are reasons for using feature scaling?

Answer: It speeds up gradient descent by making it require fewer iterations to get to a good solution.
