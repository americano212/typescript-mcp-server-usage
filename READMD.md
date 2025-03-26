```bash
docker build -t mcp/test -f ./Dockerfile .
```

```json
{
  "mcpServers": {
    "tester": {
      "command": "docker",
      "args": ["run", "-i", "--rm", "mcp/test"],
      "env": {
        "TEST": "test"
      }
    }
  }
}
```
