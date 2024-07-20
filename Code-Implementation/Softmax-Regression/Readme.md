The code is from CMU 10714(Deep Learning System)'s homework, and I have attached the homework description with code related.

## How to run the code
Training softmax regression:
```python
python3 src/simple_ml.py  
```
Testing all functions:
```
python3 -m pytest tests/test_simple_ml.py       
```
Testing a single function:
```python
 python3 -m pytest -k "softmax_loss" tests/test_simple_ml.py
```
```python
 python3 -m pytest -k "softmax_regression_epoch and not cpp" tests/test_simple_ml.py
```
 > The `-k` option in `pytest` is used to filter tests based on the names of the test functions, test class names, and test file names. It uses a substring match to select tests. When you specify `-k "softmax_regression_epoch and not cpp"`, `pytest` is selecting tests that match the following criteria:
 > 1.  **Contain `softmax_regression_epoch`**: Any test function, test class, or test file that contains the substring `softmax_regression_epoch`.
 > 2.  **Do not contain `cpp`**: Any test function, test class, or test file that does not contain the substring `cpp`.
>
>This filter is a logical combination, where the `and` operator means that both conditions must be satisfied, and the `not` operator negates the second condition.
