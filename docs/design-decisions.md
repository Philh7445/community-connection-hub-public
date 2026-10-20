# Design Decisions

[Back to the README](../README.md)

## Start with the group, not a long feature list

The project is organized around what the group wants to do: find information, talk, support one another, share useful resources, and have fun.

Keeping that purpose visible helps distinguish a helpful addition from complexity that makes participation harder.

## Keep the public description focused on shared life

The portfolio uses neutral, descriptive language about a small group of men staying connected. Friendship, learning, mutual support, and enjoyment explain the purpose without exposing the live community's identity or making a religious framing necessary.

An anonymized portfolio can explain the work without showing member conversations or identifying people.

## Combine practical areas with a playful space

Announcements and events answer practical questions. Comments make room for a response. The library gives recommendations a home. The illustrated clubhouse brings personality and fun into the experience.

Together, those areas support a community rather than just a noticeboard.

## Separate email confirmation from membership approval

Email confirmation and administrator approval serve different purposes. Email confirmation is part of signup; an administrator still decides whether the account belongs in the group.

The pending-request list makes the work visible, while explicit approve and decline actions keep the membership decision with an administrator.

## Treat mobile use as part of the core experience

A member should be able to check the site in a short visit from a phone. The mobile-friendly layout and Home Screen installation support that use.

Actual device testing matters. The iPhone unread badge, for example, can behave differently in the background than it does while the site is open. That limitation belongs in the documentation rather than being hidden behind a general claim that notifications work.

## Let members choose notifications

Notifications are opt-in. A five-minute per-device alert cooldown reduces the frequency of interruptions during active conversations.

The tradeoff is timeliness: a background badge may lag during the cooldown. Alerts and badge counts should be treated as helpful indicators, not a reliable channel for urgent information.

## Keep the library link-based

Books and external video or article links are enough to support recommendations without turning the site into a media-hosting platform.

Direct video and general-file uploads remain outside the current scope. A shared link also does not grant permission to copy or redistribute the linked work.

## Make the photo boundary explicit

Photo sharing uses a preview, pre-post removal, and a required public-sharing acknowledgement. Approved membership controls uploading, while the resulting photos are publicly accessible.

That distinction is a material limitation. A member-only conversation may contain a photo whose visibility is broader than the conversation itself. Public documentation and member guidance should say this plainly.

Photo processing accepts JPG or PNG files up to 10 MB and stores compressed JPEG images no larger than 1 MB. These size limits constrain individual images; they do not establish a total storage limit or a guaranteed cost ceiling.

## Keep the technical overview honest

The verified service responsibilities are:

- Cloudflare Workers provides the frontend and API.
- Cloudflare R2 stores photos separately.
- Supabase provides authentication and the database.

This overview deliberately stops short of claiming particular database policies, encryption guarantees, backup arrangements, retention periods, or security certifications. Those details would require a separate review of the implementation and configuration.

## Document AI assistance and human direction

Development was iterative and AI-assisted. I led the product direction and testing, including deciding what the community needed and reviewing how the result behaved in use.

That process is part of the project story. It should not be presented as entirely hand-written software or as a substitute for an independent security review.
