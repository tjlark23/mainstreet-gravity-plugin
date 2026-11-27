---
name: local-roundup
description: Answer questions about what is happening in a local market from mainstreet gravity data, such as events this weekend, new businesses, open jobs, deals or recent stories. Use when the person asks what is going on in their town or wants a short list for a newsletter or social post.
---

# Local roundup

Answer from the brand's own data in mainstreet gravity, not from memory.

1. Pick the brand. Call `list_brands` when more than one is connected and ask which town or brand they mean if it is unclear.
2. Read the right list:
   - Events: `list_events` (then `get_event` for details such as time, place and price).
   - Businesses and places: `list_businesses` or `browse_places`, then `get_business`.
   - Jobs: `list_jobs` or `browse_jobs`, then `get_job`.
   - Stories: `list_articles`, then `get_article`.
3. Keep it short. Give the few items that fit what they asked, each with its date, place and link when the tool returns one.
4. Offer the next step. If they want the list in a newsletter, use the newsletter-draft skill. If they want it saved as a story, use the article-draft skill.

If the tools return nothing for the dates or place asked, say so plainly and suggest a wider range.
