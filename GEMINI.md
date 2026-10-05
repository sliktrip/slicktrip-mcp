# SlickTrip

SlickTrip finds live flight, hotel and seat prices, links to the sellers, and alerts travelers when prices or seats change.

- Flights: `search_flights` (a round trip returns outbounds; `search_return_flights` completes it), `price_calendar` for the cheapest days, `booking_options` for sellers and checkout links.
- Hotels: `search_hotels`, `hotel_details`, `hotel_booking_options`, `hotel_price_calendar`.
- Seats: `seat_availability`, then `track_seats`.
- Alerts: `track_flight`, `track_hotel`, `add_flight_bucket_list`, `add_hotel_bucket_list`.
- Unsure of a place? Call `find_places` first.

Search with what the traveler said and never invent a place or date; ask when one is missing. Confirm with the traveler before any track_, add_, update_, stop_ or remove_ call.
