## Module for parse config file

### Example of config file
```yaml
  env: "local"
  storage_path: "./storage/storage.db"
  http_server:
    address: "localhost:7777"
    timeout: 4s
    idle_timeout: 60s
```
### Example of usage
```go
    package main

    import "github.com/quibex/config"

    func main() {
        cfg := config.MustLoad()
        ...
    }
```