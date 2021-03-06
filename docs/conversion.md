# Type Conversion Functions

The following type conversion functions are provided by Sprig:

- `atoi`: Convert a string to an integer
- `float64`: Convert to a float64
- `int`: Convert to an `int` at the system's width.
- `int64`: Convert to an `int64`
- `toString`: Convert to a string
- `toStrings`: Convert a list, slice, or array to a list of strings.
- `toBool`: Convert 1, t, T, TRUE, true, True, 0, f, F, FALSE, false, False to a boolean.

Only `atoi` requires that the input be a specific type. The others will attempt
to convert from any type to the destination type. For example, `int64` can convert
floats to ints, and it can also convert strings to ints.

## toStrings

Given a list-like collection, produce a slice of strings.

```
list 1 2 3 | toStrings
```

The above converts `1` to `"1"`, `2` to `"2"`, and so on, and then returns
them as a list.
