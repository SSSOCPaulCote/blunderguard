# blunderguard
A sentinel error package in Go as described by [Dave Cheney](https://dave.cheney.net/tag/error-handling)

# Usage

Blunderguard is very simple
```go
import (
    "fmt"

    bg "github.com/SSSOC-CAN/blunderguard"
)

const (
    ErrInvalidAction = bg.Error("invalid action")
)

func DoSomething() error {
    return ErrInvalidAction
}

func main() {
    err := DoSomething()
    if err == ErrInvalidAction {
        fmt.Println("There you go")
    }
}
```
Now your errors are immutable, fungible and constants.