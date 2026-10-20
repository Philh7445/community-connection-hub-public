# Security Overview

[Back to the README](../README.md)

Security is part of the project design, especially because the site includes member conversations and support requests. This overview describes verified controls and their limitations. It is not a formal security assessment or a guarantee that the site is free of vulnerabilities.

## Implemented controls

### Email confirmation and membership approval

Signup includes email confirmation and a separate administrator approval step. Confirming an email address alone does not grant approved membership.

Pending membership requests appear in an administrator list, with explicit approve and decline actions. Displaying a request does not approve it automatically.

These steps help control admission to the group. They do not prove a person's real-world identity or prevent every form of account misuse.

### Authenticated member access and roles

Member areas require authenticated, approved membership. The application distinguishes member and administrator roles, with administrators responsible for membership decisions.

Authentication, membership approval, and administrator authority are different concerns. The existence of those roles should not be presented as proof that every possible access-control scenario has been independently tested.

### Separate treatment of member data and photos

Member conversations are access-controlled. Photo uploads have a different visibility model:

- Uploading is limited to approved members.
- Uploaded photos are intentionally publicly accessible.
- A public-sharing acknowledgement is required before posting a photo.
- Members can preview and remove a selected attachment before posting.

Public photo access is an intentional boundary, not a claim of private media storage. A member-only page can contain an image that is accessible outside that page. Photos should therefore be suitable for public access.

### Upload format and size handling

The upload flow accepts JPG and PNG source images up to 10 MB and stores compressed JPEG images no larger than 1 MB. Direct video and general-file uploads are not supported.

These restrictions and image processing define the supported upload surface. They should not be described as a verified malware scan, guaranteed removal of hidden metadata, or protection against every malicious file.

### Generic, optional notifications

Notifications for new posts in the main conversation area are opt-in and use generic notification content. Generic wording reduces exposure of community content outside the app, such as in a device notification.

A five-minute per-device cooldown limits alert frequency. It is a notification behavior, **not** a verified security rate limit for logins, API calls, or uploads. Notifications and unread badges are not guaranteed to update in real time.

## What has not been established

This documentation does not claim:

- An independent security audit or penetration test.
- End-to-end encryption or particular encryption-at-rest arrangements.
- Multi-factor authentication.
- Verified backup, recovery, retention, or security-monitoring arrangements.
- Comprehensive abuse prevention or security rate limiting.
- A legal, privacy, or security compliance certification.

Using established infrastructure services does not, by itself, establish that every application setting or access policy is correct.

## Recommended review areas

The following are review recommendations, not descriptions of additional controls already implemented:

1. **Authorization:** Verify server-side and database access for pending, approved, declined, and administrator accounts, including attempts to reach member data directly.
2. **Media visibility:** Recheck the public-photo boundary and acknowledgement wording against how members actually understand them.
3. **Upload handling:** Review file validation, processing failures, metadata behavior, and abuse controls before making stronger upload-safety claims.
4. **Account and session handling:** Review recovery, session expiry, administrator access, and options for additional authentication protection.
5. **Operations:** Establish and test appropriate backup, recovery, logging, dependency-maintenance, and incident-response practices before documenting them as safeguards.
6. **Public release hygiene:** Check files and repository history for secrets, member information, and live deployment identifiers before publishing.

See [Privacy and safety](privacy-and-safety.md) for member guidance and the public-documentation checklist.
