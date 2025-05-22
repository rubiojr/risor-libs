# Global Functions

## exit_if_fatal

Exit the program if __fatal is true 

### Returns

No return information available.

### Example

```go
// Example usage of exit_if_fatal
exit_if_fatal()
```

## print_ok

Print a message in green. 

### Parameters

- desc: The test description

### Returns

No return information available.

### Example

```go
// Example usage of print_ok
print_ok(desc)
```

## print_fail

Print a message in red. 

### Parameters

- desc: The test description

### Returns

No return information available.

### Example

```go
// Example usage of print_fail
print_fail(desc)
```

## is_true

Assert that a condition is true. 

### Parameters

- desc: The test description
- cond: The condition to check (boolean)

### Returns

No return information available.

### Example

```go
// Example usage of is_true
is_true(desc, cond)
```

## is_false

Assert that a condition is false. 

### Parameters

- desc: The test description
- cond: The condition to check (boolean)

### Returns

No return information available.

### Example

```go
// Example usage of is_false
is_false(desc, cond)
```

## equals

Assert that two values are equal. 

### Parameters

- desc: The test description
- o1: First value to compare
- o2: Second value to compare

### Returns

No return information available.

### Example

```go
// Example usage of equals
equals(desc, o1, o2)
```

## raises

Assert a condition raises an error. 

### Parameters

- desc: The test description
- fn: The function that should raise an error
- err: The error that should be raised (default: any error)

### Returns

No return information available.

### Example

```go
// Example usage of raises
raises(desc, fn, err="")
```

## nothing_raised

Assert a condition does not raise an error. 

### Parameters

- desc: The test description
- fn: The function that should not raise an error

### Returns

No return information available.

### Example

```go
// Example usage of nothing_raised
nothing_raised(desc, fn)
```

## stdout_equals

Assert that command output equals an expected string. 

### Parameters

- desc: The test description
- cmd: The command to run
- expected: The expected output

### Returns

No return information available.

### Example

```go
// Example usage of stdout_equals
stdout_equals(desc, cmd, expected)
```

## stderr_matches

Assert that command stderr output matches a regular expression. 

### Parameters

- desc: The test description
- cmd: The command to run
- reg: The regular expression to match

### Returns

No return information available.

### Example

```go
// Example usage of stderr_matches
stderr_matches(desc, cmd, reg)
```

## stdout_matches

Assert that command output matches a regular expression. 

### Parameters

- desc: The test description
- cmd: The command to run
- reg: The regular expression to match

### Returns

No return information available.

### Example

```go
// Example usage of stdout_matches
stdout_matches(desc, cmd, reg)
```

## is_dir

Assert that a path is a directory. 

### Parameters

- desc: The test description
- path: The path to check

### Returns

No return information available.

### Example

```go
// Example usage of is_dir
is_dir(desc, path)
```

## is_file

Assert that a path is a file. 

### Parameters

- desc: The test description
- path: The path to check

### Returns

No return information available.

### Example

```go
// Example usage of is_file
is_file(desc, path)
```

## with_temp_dir

Create a temporary directory and run a function with it. The directory created is automatically removed after the function is run. 

### Parameters

- fn: The function to run with temporary directory path as argument

### Returns

The result of the function execution

### Example

```go
// Example usage of with_temp_dir
with_temp_dir(fn)
```
