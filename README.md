# grscheller-docs

Detailed
[documentation](https://grscheller.github.io/grscheller-pypi-namespace-docs/)
for all the currently maintained grscheller namespace projects on PyPI.

Corresponding GitHub source code repos:

* [grscheller.boring-math](https://github.com/grscheller/boring-math)
* [grscheller.circular-array](https://github.com/grscheller/circular-array)
* [grscheller.datastructures](https://github.com/grscheller/datastructures)
* [grscheller.experimental](https://github.com/grscheller/experimental)
* [grscheller.fp](https://github.com/grscheller/fp)

Using the grscheller.boring-math as an example, here is how one
generates the docs with pdoc. The boring-math project depends on both
the fp and circular-array projects.

```bash
   $ cd docs/boring_math/API/development/
   $ rm -r grscheller/ index.html search.js
   $ PYTHONPATH=~/devel/pypi/circular-array/src:~/devel/pypi/fp/src:~/devel/pypi/boring-math/src
   $ pdoc -o . grscheller.boring_math
```

