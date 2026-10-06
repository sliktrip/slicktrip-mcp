# Installing SlickTrip (for AI agents)

SlickTrip is a hosted remote MCP server. There is nothing to clone, build or run; do not install packages.

1. Add a remote MCP server named `slicktrip` with URL `https://mcp.slicktrip.com/mcp` (transport: streamable HTTP).

   For clients that read a JSON config (Cline's `cline_mcp_settings.json`, Cursor's `mcp.json`, and similar):

   ```json
   {
     "mcpServers": {
       "slicktrip": {
         "type": "streamableHttp",
         "url": "https://mcp.slicktrip.com/mcp"
       }
     }
   }
   ```

   Use `"type": "http"` instead if the client rejects `streamableHttp`.

2. On first use the server asks for OAuth sign-in (OAuth 2.1 with PKCE and dynamic client registration; discovery at `https://mcp.slicktrip.com/.well-known/oauth-authorization-server`). Open the sign-in page it gives you and sign in or create a free SlickTrip account with Google, Apple or email. No API key is needed.

3. Check the connection by listing tools: you should see `search_flights`, `price_calendar`, `search_hotels`, `seat_availability`, `track_flight` and more (35 in all).

Try: "Cheapest nonstop from New York to Lisbon in March, one week."

Setup guide: https://slicktrip.com/connector · Support: support@slicktrip.com
