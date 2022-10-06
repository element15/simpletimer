# `simpletimer`

This utility provides a user-friendly wrapper around Python's `perf_counter()` for timing sections of code and printing the results to the terminal.

```Python
from simpletimer import tic, toc

# Record the start time
t = tic('Started the timer...')

# Do something that takes time to complete
foo = ['spam and eggs'] * 10_000

# Calculate the elapsed time and print the result
toc(t)
```

```
[2022-10-06T16:04:59] Started the timer...done. 415.5 µs
```

## Installation
```
python3 -m pip install --user git+https://github.com/element15/simpletimer
```

## Documentation

This utility consists only of two functions, `tic` and `toc`, which effectively start and stop the timer, respectively. Calling `tic` returns a timestamp value which will need to be supplied to `toc` to calculate elapsed time.

More information on the arguments that can be passed to `tic` and `toc` are available in the docstrings. To view them, type `help(tic)` or `help(toc)`.
