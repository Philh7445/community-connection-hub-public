# Roadmap and Review Priorities

[Back to the README](../README.md)

This page separates a proposed feature from working functionality. It is not a release schedule or a promise that every idea will be implemented.

## Proposed feature: library collections

A named collection could bring several resources together around an interest or topic.

The proposed collection would support an ordered mix of:

- Books.
- Video links.
- Article or other web links.

For example, a clearly fictional collection called **Learning Something New** could contain a recommended book, an introductory video, and a related article in a useful reading and viewing order.

### Questions to resolve before implementation

- Who can create or edit a collection?
- How should resources be added and reordered on a phone?
- Can the same resource appear in more than one collection?
- What should happen when a linked resource becomes unavailable?

**Status:** Proposed. Mixed, ordered collections are not implemented and must not appear in the current-feature list as working functionality.

## Suggested review priorities

These are areas worth reviewing as the project develops, not claims that additional functionality already exists or has been scheduled.

### Mobile clarity

Continue testing important flows on actual devices, with attention to installation, photo previews, and the difference between in-app unread state and background badge updates.

### Public-photo understanding

Review the wording and placement of the photo acknowledgement so members understand the visibility boundary before posting. Any future move to access-controlled media would be a separate design and implementation change, not something this documentation assumes is already available.

### Accessibility and ease of use

Review navigation, readable text, interaction labels, and non-pointer access to the illustrated clubhouse. No accessibility audit or compliance certification is claimed.

### Operating costs

Review hosting, storage, and delivery usage as the site grows. Per-image compression is useful, but a fixed cost cap should not be promised without an actual mechanism that enforces it.

## Out of current scope

- Public membership or broad social-network features.
- Direct video hosting.
- General-purpose document and file uploads.
- Claims of confidential media storage under the current public-photo design.

The priority remains a manageable, useful place for a small group to stay connected.
