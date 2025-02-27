Download link :https://programming.engineering/product/math-6490-nonlinear-optimization-in-machine-learning-assignment-3/

# MATH-6490.-Nonlinear-Optimization-in-Machine-Learning.-Assignment-3.
MATH 6490. Nonlinear Optimization in Machine Learning. Assignment 3.
There are 3 problems, each problem is worth 5 points, total is 15 points.

1. Let f(x) =

1

xT Qx bT x + c as we introduced in Theorem 4.1 in the Lecture

2

Notes. Here Q 0 is a positively de nite symmetric matrix such that its eigenvalues satisfy 0 < m = n n 1 ::: 1 = L < 1, where m and L are the strong{ convexity constant for f and the Lipschitz constant for rf. Show that rf = Qx b. Then show that min f(x) = f(x ) where x is the unique solution of the linear equation

Qx

x

b = 0.

2. Following problem 1. Let the dimension n = 2. Consider the matrix

T =“(1+ )(II Q) (I0

Q)#

that we introduced in Theorem 4.1 in the Lecture Notes. According to standard linear

algebra, there exist an orthogonal matrix U of size 2 2 such that UT QU = “

0

#

01

2

. De ne the permutation matrix

03

2

1

0

0

7

600107

= 6

0 1

0 07

:

6

7

5

0001

Show that

“

#T

“

#

U

0

U

0

0

U

T

T = diag(T1; T2) ;

0

U

#

where each block Ti =

“(1 +

1

i

)

0

i

for i = 1; 2.

)(1

(1

)

(Hint: One rst easily sees that

“

0 U#

T

T

“0 U#

=

“

I

0

#

R :

U 0

U 0

(1+ )(I)

(I)

The fact that R T = diag(T1; :::; Tn) follows from standard row and column transfor-


mations. Indeed we have

2(1 +

)(1

)

0

(1

)

0

3

0

1

(1 + )(1

2)

0

1

(1

2)

6

1

0

0

0

7

6

7

6

0

1

0

0

7

6

7

4

5

(1 + )(1

)

(1

)

0

0

3

permute column 2 and 3 2

0

1

0

1

(1 + )(1

2)

(1

2)

;

!

6

1

0

0

0

7

6

7

6

0

0

1

0

7

6

7

4

5

(1 + )(1

)

(1

)

0

0

3

permute row 2 and 3

2

1

1

0

1

0

2)

(1

0

!

6

0

0

(1 + )(1

2)

7

6

7

6

0

0

1

0

7

6

7

as desired.)

4

5

3. Show that if the sequence k 0, 0 = 0 is de ned recursively by

k2 =

(1

2)2

k

;

(1

2

1

)2

k

then

2

1

k2

:

k + 2

This yields the convergence rate

f(xk) f

C

kxk

x k2

(k + 1)2

as we demonstrated in the Nesterov’s optimal algorithm Algorithm 4.3 in the Lecture

Notes.

2

(Hint: Do this by induction. For k = 0 we have 1 02

= 1

0 = 1

.

0 + 2

Suppose for some k we have 1

k2

2

. We aim to show that 1

k2

+1

2

.

k + 2

k + 3

Suppose this is not the case, so that 1

2

>

2

. Then 2

< 1

2

=

k + 1

,

k+1

k + 3

k+1

k + 3

k + 3

1

k + 3

i.e.,

>

. Then using the recursive relation we see that

2

k + 1

k+1

4

(1 k2)2 =

(1 k2+1)2

>

2

2

k + 3

=

4

:

(k + 2)2

k + 3

k2

+1

k + 1 (k + 1)(k + 3)

This leads to (k + 1)(k + 3) > (k + 2)2, which is same as 3 > 4, that is a contradiction.)
