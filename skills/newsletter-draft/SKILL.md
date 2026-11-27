---
name: newsletter-draft
description: Build or update a draft issue of a local newsletter in mainstreet gravity. Use when the person asks to start, fill, edit or check next week's newsletter, an issue, a section, the intro or the subject line.
---

# Build a newsletter draft

Work only through the mainstreet gravity tools. Every change stays in a draft; nothing here sends or schedules an issue.

1. Find the newsletter. Call `list_brands` if more than one brand is connected, then `list_publications` and `list_issues`.
2. Start or open the issue. Use `create_issue` from the newsletter's template for a new one, or `get_issue_tree` to read an existing draft before changing it.
3. Fill it. For a whole issue, `generate_issue` has the brand's own writer draft every section. For one section, use `browse_content`, `browse_places` or `browse_jobs` to find real local items, then `add_story`, `add_event`, `add_job` or `write_story_for_section`.
4. Polish. `write_intro`, `suggest_subject_lines` and `update_issue_details` set the opening, subject line and preview text. `update_block_text` changes one block's words.
5. Check. Run `review_issue`, then `get_review`, and fix what it flags.
6. Hand it back. Tell the person the issue is ready for them to look over in mainstreet gravity. Sending, scheduling and pushing to an email platform are the person's call: only use `push_to_beehiiv` or `push_to_activecampaign` when they ask for it in this conversation.

Use only items the tools return. If a section has nothing real to say this week, leave it empty and say so rather than inventing an item.
