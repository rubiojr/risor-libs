# Global Functions

## log

Logs a message to standard output

### Parameters

- msg: The message to log

### Returns

No return information available.

### Example

```go
// Example usage of log
log(msg)
```

## debug

Logs a debug message when RSX_DEBUG environment variable is set to "1"

### Parameters

- msg: The debug message to log

### Returns

No return information available.

### Example

```go
// Example usage of debug
debug(msg)
```

## shell

Executes a shell command and returns its output

### Parameters

- command: The shell command to execute

### Returns

The combined stdout and stderr output as a string

### Example

```go
// Example usage of shell
shell(command)
```

## sh

Alias for shell function

### Parameters

- command: The shell command to execute

### Returns

The combined stdout and stderr output as a string

### Example

```go
// Example usage of sh
sh(command)
```

## env

Gets an environment variable with a default value

### Parameters

- key: The environment variable name
- def: The default value if the variable is not set

### Returns

The value of the environment variable or the default value

### Example

```go
// Example usage of env
env(key, def)
```

## is_file

Checks if a path is a file

### Parameters

- target: The path to check

### Returns

Boolean indicating whether the target is a file

### Example

```go
// Example usage of is_file
is_file(target)
```

## is_dir

Checks if a path is a directory

### Parameters

- target: The path to check

### Returns

Boolean indicating whether the target is a directory

### Example

```go
// Example usage of is_dir
is_dir(target)
```

## lines

Splits content into lines, handling both strings and files

### Parameters

- content: A string or file path to split into lines

### Returns

An array of lines

### Example

```go
// Example usage of lines
lines(content)
```

## replace_in

Replace occurrences of a regular expression in a file or string

### Parameters

- target: The file path or string to process
- rgxp: The regular expression pattern to match
- repl: The replacement string

### Returns

The modified content as a string

### Example

```go
// Example usage of replace_in
replace_in(target, rgxp, repl)
```

## grep

Find lines in a file or string that match a regular expression

### Parameters

- target: The file path or string to search
- regex: The regular expression pattern to match

### Returns

An array of matching lines

### Example

```go
// Example usage of grep
grep(target, regex)
```
