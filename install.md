# HubSpot MCP Configuration

Add the following configuration to your `claude_desktop_config.json` file:

```json
"HubSpot": {
  "command": "uv",
  "args": [
    "run",
    "--with",
    "mcp>=1.4.1",
    "--with",
    "hubspot-api-client>=11.1.0",
    "--with",
    "python-dotenv>=1.0.1",
    "python",
    "/your-cloned-directory/mcp-hubspot/src/mcp_server_hubspot/server.py"
  ],
  "env": {
    "HUBSPOT_ACCESS_TOKEN": "your-access-toksn"
  }
}
```

Make sure to:
1. Verify the path to the server.py file is correct for your system
2. Use your own HubSpot access token if needed
3. Ensure all required dependencies are installed