# Code as Data: a Practical Introduction to Python's Abstract Syntax Tree

Slides and some code for my PyData Paris 2025 talk.

## Objective

My goal was to demystify the concept of abstract syntax trees (AST).  
The name is a bit scary, and it often comes up in conversations on topics (compilers, interpreters) that might not be familiar to all software engineers.

But it's not that hard to get started and benefit from the magic of AST manipulation.

## Code

The code in `assert_transform.py` shows the code presented in the slides as a 'proof of concept' of a transform to achieve a pytest-like experience.  
It is a bit simplistic - to fit on slides and focus the discussion - but the principle is there.

`python assert_transform_pytest.py` shows the result of pytest assertion rewriting.

Tested with Python 3.11. 

## References

On pytest using AST transforms:

- [pytest blog post](http://pybites.blogspot.be/2011/07/behind-scenes-of-pytests-new-assertion.html)
- A relevant part of [pytest source code](https://github.com/pytest-dev/pytest/blob/be83aa618c68ebb9080b537bbd8b19b97a7f4eb8/src/_pytest/assertion/rewrite.py#L615">https://github.com/pytest-dev/pytest/blob/be83aa618c68ebb9080b537bbd8b19b97a7f4eb8/src/_pytest/assertion/rewrite.py#L615)

General resources:

- [Unofficial AST docs](https://greentreesnakes.readthedocs.io/en/latest/)
- [https://eli.thegreenplace.net/2009/11/28/python-internals-working-with-python-asts](https://eli.thegreenplace.net/2009/11/28/python-internals-working-with-python-asts)
This is a fantastic blog, and these 'old' blog posts are still relevant.
- An AST talk I enjoyed: [video](https://www.youtube.com/watch?v=XhWvz4dK4ng), [slides](https://emilyemorehouse.github.io/ast-and-me/) by Emily Morehouse-Valcarcel.
- The blossom tree in the slides is inspired by [this famous talk from Victor Bret](https://www.youtube.com/watch?v=PUv66718DII)
