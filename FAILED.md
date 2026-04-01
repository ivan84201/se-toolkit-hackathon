❌ Full stack working: Flutter serves content, WebSocket accepts, agent responds
    -> The full chain must work end-to-end: 1. Flutter at /flutter must serve real content (main.dart.js present). 2. WebSocket at /ws/chat must accept connections with the correct NANOBOT_ACCESS_KEY. 3. The agent must respond through the WebSocket without LLM errors. Common issues: entrypoint env var names must match docker-compose.yml, Caddyfile routes must be uncommented, flutter volume must be mounted in caddy.
    Details: SSH root@10.93.26.55: command exited with 2 (expected 0). Output: error: Failed to generate package metadata for `nanobot==0.1.0 @ virtual+nanobot`
  Caused by: Failed to parse entry: `mcp-webchat`
  Caused by: `mcp-webchat` is included as a workspace member, but re