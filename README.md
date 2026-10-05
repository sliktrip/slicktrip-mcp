<img src="assets/logo.png" width="72" alt="SlickTrip">

# SlickTrip for AI assistants

Live flight, hotel and seat prices, cheapest-day calendars, and price-drop and seat alerts, inside your AI assistant.

SlickTrip is a hosted remote MCP server. This repository holds only the plugin and extension manifests that point at it; there is nothing to install or run locally.

**Server:** `https://mcp.slicktrip.com/mcp` (streamable HTTP, OAuth 2.1 with PKCE and dynamic client registration)
**Registry:** `com.slicktrip/slicktrip` in the [official MCP Registry](https://registry.modelcontextprotocol.io)

## What you can ask

- "Cheapest nonstop from New York to Lisbon in March, one week."
- "Which days in November are cheapest to fly Chicago to Denver?"
- "Is there an aisle seat left on AA100 on the 20th?"
- "Hotels near the Colosseum under $250 a night, and watch the price."
- "Alert me when any flight to Tokyo drops under $700 this spring."

Alerts and saved lists use a free SlickTrip account (Google, Apple or email); some assistants ask you to sign in when you connect. Booking completes on the seller's site.

## Install

| Client | How |
| --- | --- |
| Claude | Settings → Connectors → browse → **SlickTrip** (in the directory) |
| ChatGPT | Apps → search **SlickTrip** |
| Cursor | Marketplace → **SlickTrip**, or add `https://mcp.slicktrip.com/mcp` as a remote MCP server |
| Claude Code | `/plugin marketplace add sliktrip/slicktrip-mcp` then `/plugin install slicktrip@slicktrip` |
| Gemini CLI | `gemini extensions install https://github.com/sliktrip/slicktrip-mcp` |
| VS Code / GitHub Copilot | MCP: Add Server → HTTP → `https://mcp.slicktrip.com/mcp` |
| Anything else that speaks MCP | Add `https://mcp.slicktrip.com/mcp` as a remote server |

Full setup guide: https://slicktrip.com/connector

## Tools

Flights (`search_flights`, `search_return_flights`, `price_calendar`, `flight_lookup`, `route_airlines`, `booking_options`), hotels (`search_hotels`, `hotel_details`, `hotel_price_calendar`, `hotel_booking_options`), seats (`seat_availability`), alerts for fares, stays, seats and flexible bucket lists (`track_*`, `add_*_bucket_list`, `list_*`, `update_*`, `stop_*`), plus `find_places`, `recent_deals`, `share_link`, and account tools.

## Links

[Privacy](https://slicktrip.com/policy) · [Terms](https://slicktrip.com/tos) · support@slicktrip.com
