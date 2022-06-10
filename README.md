# blunderguard
A sentinel error package in Go as described by [Dave Cheney](https://dave.cheney.net/tag/error-handling)

# Usage

Blunderguard is very simple
```go
import (
    bg "github.com/SSSOC-CAN/blunderguard"
)

const (
    ErrInvalidAction = bg.Error("invalid action")
)
```
Now your errors are immutable, fungible and constants.