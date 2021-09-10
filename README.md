# L03E02: Matrix multiplication
Vytvořte balíček `argebra` obsahující dva moduly `matrix.py` a `vector.py`.

Modul `vector.py` obsahuje funkci `dot_product(vector_1, vector_2)`, která počítá [skalární součin](https://www.matweb.cz/skalarni-soucin) dvou stejně dlouhých vektorů (vektor reprezentujeme jako seznam).

Například tedy:

```python
from algebra.vector import dot_product

vector_1 = [1, 2, 3]
vector_2 = [3, 2, 1]

assert dot_product(vector_1, vector_2) == 10
```

Modul `matrix.py` obsahuje funkci `matrix_multiplication(matrix_1, matrix_2)` vykonávající [násobení dvou matic] (https://cs.wikipedia.org/wiki/Násoben%C3%AD_matic). V implementaci využíjte funkci `algebra.vector.dot_product()`. Matice můžete reprezentovat jako seznam (mutovatelnost se nám již hodí).

Například tedy:

```python
from algebra.vector import dot_product

matrix_1 = [
    [1, -2, 5, 20],
    [0, 2, 3, 4],
    [100, 2, 3, 4]
]

matrix_2 = [
    [10, -2],
    [0, 20],
    [100, 2],
    [2, 10]
]

assert matrix_multiplication(matrix1, matrix2) == [[550, 168], [308, 86], [1308, -114]]
```
