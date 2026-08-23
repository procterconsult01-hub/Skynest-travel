# SkyNest — Real Booking API Integration Plan

## Goal
Move from “search + redirect” to live flight & hotel results displayed on SkyNest, with optional direct booking or deep links.

## Recommended Providers (2026)

### Flights
| Provider       | Strengths                          | Pricing model          | Best for          |
|----------------|------------------------------------|------------------------|-------------------|
| **Duffel**     | Modern API, great docs, NDC        | Pay-per-booking + %    | Startups          |
| **Amadeus**    | Largest inventory, self-service    | Free tier + paid       | Scale             |
| **Travelport** | Strong GDS                         | Enterprise             | High volume       |
| **Kiwi Tequila**| Virtual interlining                | Revenue share          | Complex routes    |

**Recommended start**: Duffel (fastest time-to-market, excellent developer experience).

### Hotels
| Provider          | Strengths                     | Notes                    |
|-------------------|-------------------------------|--------------------------|
| **Booking.com Affiliate** | Huge inventory, easy     | Deep links + commission  |
| **Hotelbeds**     | B2B rates                     | Good for packages        |
| **Amadeus Hotel** | Unified with flights          | Convenient               |

## Phased Rollout

### Phase 1 — Live Search (4–6 weeks)
- Integrate Duffel Flight Search API
- Display results in a clean results page (price, airline, duration, stops)
- Keep “Book on airline site” button (deep link or Duffel order)
- Cache popular routes aggressively

### Phase 2 — Hotel Results (3–4 weeks)
- Add Booking.com Affiliate API or Hotelbeds
- Unified search results (flights + hotels side-by-side for packages)

### Phase 3 — Booking Flow (6–8 weeks)
- Optional: complete booking via Duffel (you become the merchant of record or use their payment)
- Or continue redirect model for lower liability

### Phase 4 — Advanced
- Price alerts (email/push)
- Multi-city & complex itineraries
- Seat maps, ancillaries
- User accounts + trip history

## Technical Stack Suggestion
- Frontend: current static site → Next.js or Astro for SSR + API routes
- Backend: Node.js / serverless (Cloudflare Workers or Vercel)
- Database: for saved searches & users (Supabase or PlanetScale)
- Caching: Redis / Cloudflare KV for fare results

## Legal & Compliance
- Obtain necessary IATA / ARC accreditation if issuing tickets
- Clear disclosure that SkyNest may earn affiliate commission
- Update Terms & Privacy
- PCI compliance if handling cards

## Estimated First-Year Cost (low volume)
- Duffel: mostly success-based
- Amadeus free tier sufficient for testing
- Hosting: still free/cheap on Cloudflare
- Total to MVP live results: <$500–1,000 + developer time

## Next Immediate Action
1. Create free developer accounts at Duffel and Amadeus
2. Prototype flight search on a /results page
3. Measure conversion from search → click-out

Contact: engineering@skynest.travel (once set up)
