# Privacy and Safety

[Back to the README](../README.md)

This page describes known boundaries and sensible publication precautions. It is not a legal privacy policy, security audit, or compliance statement.

## Two different access boundaries

### Membership-controlled access

Signup includes email confirmation and administrator approval. Member and administrator roles distinguish ordinary participation from membership management.

Member conversations are access-controlled. This describes the intended and implemented membership boundary, not a guarantee against every security risk.

### Publicly accessible photos

Approved members can upload photos, but the stored photos are intentionally publicly accessible. The posting flow requires an acknowledgement of that visibility.

A private conversation and a photo attached to it do not necessarily have the same audience. A person with access to a photo URL may be able to view the photo without having access to the conversation.

**Do not describe the whole site or all of its media as private.**

## Practical guidance for members

- Only post photos that are appropriate to be publicly accessible.
- Get permission from people pictured before sharing an image of them.
- Avoid images that expose personal documents, addresses, account details, or other sensitive information.
- Remember that other people may copy an accessible image. A later removal cannot be assumed to retrieve copies already made elsewhere.
- Use support requests thoughtfully and avoid sharing someone else's sensitive personal details without permission.

Support requests and community notifications are not an emergency service. The site should not be relied on for urgent assistance or guaranteed immediate delivery.

## Preview and removal have a specific meaning

The confirmed photo flow supports previewing and removing a selected attachment **before posting**.

That should not be expanded into claims about deletion of published photos, retention schedules, automatic removal of copies, or image-metadata stripping. Those behaviors are not established by this documentation.

## Resource-sharing boundaries

The library shares recommendations and external links. It does not imply permission to copy books, articles, or videos into the project or to redistribute someone else's work.

Public examples should use fictional recommendations or material whose inclusion is appropriate, without revealing members' personal reading or viewing activity.

## What belongs in a public portfolio

Appropriate material includes:

- An anonymized explanation of the need and intended audience.
- General feature descriptions and known limitations.
- A high-level account of the technology and development process.
- Clearly labeled fictional examples or purpose-made mockups, if added later.

The public repository should omit:

- The live community's name and domain.
- Member names, email addresses, account identifiers, and contact details.
- Private URLs, invitation links, access tokens, credentials, and configuration secrets.
- Actual member posts, support requests, photographs, or screenshots of private content.
- Private jokes or distinctive details that identify individual people.
- Private source code or deployment configuration not separately approved for publication.

This documentation pack contains no live screenshots or private source code.

## Before publishing or adding new material

- [ ] Review every file for identifying details and live-service links.
- [ ] Keep current features and proposed additions separate, and preserve the public-photo warning.
- [ ] Use clearly fictional demonstrations and confirm permission and licensing for any code or assets added later.
- [ ] Inspect repository history as well as current files. Deleting a file from the latest revision does not necessarily remove it from earlier commits.
- [ ] If a secret has ever been exposed, address the exposure and rotate it rather than assuming deletion alone is enough.
- [ ] Verify implementation details before adding claims about retention, backups, encryption, accessibility, or security controls.

## Limits of these notes

This documentation does not establish legal compliance, a completed security assessment, guaranteed privacy, or a fixed hosting cost. A deployment intended for another group would need its own review of access controls, media visibility, service configuration, permissions, and operating requirements.
