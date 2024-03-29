[![Downloads](https://static.pepy.tech/badge/precreal)](https://pepy.tech/project/precreal) [![Downloads](https://static.pepy.tech/badge/precreal/month)](https://pepy.tech/project/precreal) [![Downloads](https://static.pepy.tech/badge/precreal/week)](https://pepy.tech/project/precreal)

This is a Python package to do exact real arithmetic, the following is an example using it:

```python
from precreal import Real,intpow,pi

>>> 0.1+0.2==0.3 # Precision loss

False

>>> Real("0.1")+Real("0.2")==Real("0.3") # The Real class has NO precision loss when doing arithmetic

True

>>> intpow(Real(2),100)

1267650600228229401496703205376

>>> pi(7)
3.1415926
```

You can also run `precreal_test`, which tests three features of this package.

changelog:

* 1.0.0 First version
* 1.0.1 Fixed a setup.py bug
* 1.0.2 Fixed the bug that pi computing results in 10 more digits