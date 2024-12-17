## Indexed Data

The key idea of indexed data is to encode type equalities in data.
When we come to inspect the data (usually, via structural recursion) we discover these equalities, which in turn limit what values we can produce. 
Notice, again, the duality with codata. 
Indexed codata limits methods we can call. 
Indexed data limits values we can produce.
Also, remember that indexed data is often known as generalized algebraic data types.
We are using the simpler term indexed data to emphasise the relationship to indexed codata,
and also because it's much easier to type!

Let's see a simple, and classic, example: evaluating a small language.
Our language will have basic arithmetic as well as conditionals, which is just enough to make it interesting.
We'll start with the version without indexed data.

```scala mdoc:silent
enum Expr {
  case Literal
}
```
