# Worker pool

Simple worker pool to run arbitrary functions concurrently.

```Go
import pool
// Create a pool with 2 workers
pool.new(2)

// Queue up some jobs
for range 10 {
  pool.queue(func() { time.sleep(1); print("hello") })
}

// Wait for all jobs to finish
pool.wait()
```
