# Scalar Go Test Go API

Complete reference of every operation, grouped by resource. See [the README](./README.md) for usage and configuration.

## Contents

- [`Ping`](#ping)
  - [Ping the API](#ping-the-api)

## Setup

```go
import (
	"context"
	"fmt"

	sdk "github.com/amritk/scalar-go"
)

client := sdk.NewClient()
```

## `Ping`

### Ping the API

| Direction | Type |
| --- | --- |
| Response | [`PingPingResponse`](./ping.go) |

```go
ping, err := client.Ping.Ping(context.Background())
if err != nil {
	panic(err)
}
fmt.Println(ping)
```
