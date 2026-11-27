---
name: article-draft
description: Write a local news article and file it as a draft for review in mainstreet gravity. Use when the person asks to turn notes, a link, a press release or a brain dump into a story for their site.
---

# File an article draft

Every article lands as a draft or in review. Publishing stays a person's decision.

1. Learn the brand's voice. Call `get_brand` and `get_writer_guide` for the brand's rules, then `list_authors` for a valid byline.
2. Gather facts. Read any link the person gives with `read_link`. Use `web_search` or `web_extract` only for facts the person asked you to look up. Use only facts you can point to.
3. Write it. For rough notes, `write_from_brain_dump` drafts a story in the brand's voice. Otherwise write the blocks yourself.
4. Check before filing. Run `check_article_draft` and fix every problem it lists.
5. File it. Call `file_article_draft` with the `externalId` the check returned. Pass `draft_only` as true unless the person asked for it to go to review.
6. Report back with the draft's status from `get_draft_status`. Use `publish_article` only when the person tells you in this conversation to publish that article.
