# Community Connection Hub

A mobile-friendly gathering place for a small group of men to stay connected, share everyday life, and enjoy time together between in-person gatherings.

## The idea

I wanted to create a place where a group could do more than exchange announcements. Members needed somewhere to keep a conversation going, share what was happening in their lives, find the next gathering, recommend a good book or video, and have a little fun along the way.

Community Connection Hub brings those activities together in one approachable website. The goal is simple: help a small community stay connected without making participation feel like another task.

This is a descriptive portfolio title. The live community's name, web address, member information, and private content are intentionally excluded from this documentation.

## What it offers

- **Community information:** Announcements and events in a shared place.
- **Ongoing conversation:** Posts and comments that help members stay in touch between gatherings.
- **Member support:** Requests, follow-up updates, and active or resolved status.
- **A resource library:** Recommended books and links to useful articles, inspirational or educational videos, and other web resources.
- **A playful clubhouse:** Clickable illustrated objects and seasonal decorations that give the site personality.
- **Photo sharing:** Image attachments with a preview and the option to remove an image before posting.
- **Mobile access:** A phone-friendly experience with Home Screen installation and optional notifications for new posts in the main conversation area.
- **Membership management:** Email-confirmation signup, administrator approval, and separate member and administrator roles.

## An important privacy distinction

Member access and conversations are membership-controlled. Uploaded photos, however, are intentionally publicly accessible. Uploading is limited to approved members, and a public-sharing acknowledgement is required before posting a photo.

The site should not be described as completely private. A membership gate does not make its photo storage private. See [Privacy and safety](docs/privacy-and-safety.md) for the boundaries and publication checklist.

## Security overview

The site combines authenticated member access, email-confirmation signup, administrator membership approval, and separate member and administrator roles. Photo uploads have defined format and size limits, and notification messages use generic content.

These controls have limits. In particular, uploaded photos are publicly accessible even though member conversations are access-controlled. No formal security audit, complete protection, or specific encryption guarantee is claimed. See the [Security overview](docs/security-overview.md) for implemented controls and areas requiring further review.

## Technology overview

The implementation uses three main services:

- **Cloudflare Workers:** Frontend and API.
- **Cloudflare R2:** Separate storage for uploaded photos.
- **Supabase:** Authentication and database.

This repository focuses on the product, its goals, and the decisions behind it. It does not include private source code, credentials, account identifiers, live member content, or deployment instructions.

## My role and approach

I led the product direction and testing. Development was iterative and AI-assisted, with changes informed by actual use and testing on real devices.

The work involved defining what the group needed, trying features in everyday situations, reviewing how they behaved, and refining the experience. These notes describe the working functionality and its known limitations, not a professional security audit or a claim of production readiness for other communities.

## Documentation

| Document | What it covers |
| --- | --- |
| [Project background](docs/project-background.md) | The original need, intended audience, and product goals |
| [Features](docs/features.md) | Working functionality, behavior, and current limits |
| [Design decisions](docs/design-decisions.md) | The reasoning behind the experience and technical choices |
| [Roadmap](docs/roadmap.md) | Proposed additions, clearly separated from implemented features |
| [Privacy and safety](docs/privacy-and-safety.md) | Access boundaries, public photos, and safe portfolio publishing |
| [Security overview](docs/security-overview.md) | Verified security controls, their limits, and recommended review areas |

## Current scope

This is a small-community project, not a general-purpose social network or a public file-sharing service. Video and article sharing uses links; direct video and general-file uploads are not supported.

Named library collections that mix and order books, videos, and articles are a proposed improvement, not a working feature. No fixed delivery schedule or guaranteed hosting-cost ceiling is claimed.

## Reuse and licensing

This documentation does not grant a software or content license. Any code, media, or other material made available for reuse would need its own clearly stated license and appropriate permissions.
