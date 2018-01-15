Some notes about Algorithm design and analisys.

To study algorithms behavior and to describe them by a mathematical point of view.
Describing algorithm by math give us a exact criteria to compare performaces.
Criterias are implemented by a mathematical model (a function) and are used to
see how an algorithm behave in the optimal case, in the average case and in it's
worst case. So an algorithm may have more than one model to describes how it behave.
<h4>Landau notation</h4>
Landau notation comes to help classify algorithm behavior. Given some functions
$f:\mathbb{N} \to \mathbb{R}$. We can say $f(n)$ is in $O(g(n))$ if
$$ \lim_{n \to \infty} \frac{f(n)}{g(n)} \lt \infty$$
$f(n)$ is in the same order of $g(n)$ means that exists constant $K$ that:
$$  \lim_{n \to \infty} \frac{f(n)}{Kg(n)} \lt 1 $$
$f(n)$ is in an order inferior than $g(n)$ if
$$  \lim_{n \to \infty} \frac{f(n)}{g(n)} \lt 0 $$
Let say $n$ is the data set size our algorithm will work on. So when we say that
an algorithm is in $O(n ln n)$ order we say that we can represent the algorithm
behavior by function $f(n)$ and generally speaking $f(n)$ behaves like $n ln n$,
performances are similar or differ by a constant factor, call it $K$.
