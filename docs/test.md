# Test

Risor library to write tests.

```Go
import test

test.is_true("this test will not fail", true)

test.raises("this test should raise a boom error", func(){
  error("boom")
}, errors.new("boom"))

test.nothing_raised("this test should raise a boom error", func(){
  true
})
```

