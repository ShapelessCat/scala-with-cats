# Tagless Final Interpreters

We've seen the duality between data and codata in many places, starting in [@sec:codata], but we haven't yet explored interpreters that use the codata approach. In this chapter we'll do so, looking at a strategy known as **tagless final**.

Tagless final is a little bit more than a straightforward application of the data-codata duality.
In particular, it solves a problem around extensibility known as the **expression problem**.
We first met this problem in [@sec:codata:extensibility].
In the context of interpreters, solving the expression problem allowing extensibility of both the programs we write and the interpreters that run them.

We'll start this chapter looking at codata interpreters.
We'll see they have a shortcoming, which motivates the expression problem.

Solving the expression problem allows for very expressive code, as the name suggests.
