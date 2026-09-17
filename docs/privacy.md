# Privacy Policy
_Last updated: 17 September 2026_

This page explains what data Migaga stores, why it stores it, and how to have it
removed. Migaga is a hobby project and is 100% open source - everything described
here can be verified in the [source code](https://github.com/LewisHobden/Migaga).

## The short version
- Migaga **does not store the content of your messages.**
- Migaga stores Discord IDs, plus anything you or your server administrators
  explicitly ask it to remember (a profile, a reminder, a welcome message).
- Nothing is sold, shared, or used to train machine learning or AI models.
- You can ask for your data to be deleted at any time, join the Discord and ping a moderator.

## What Migaga stores

### Discord identifiers
Migaga stores numeric Discord IDs - user IDs, server IDs, channel IDs, role IDs,
message IDs and emoji IDs - so that it can associate its features with the right
people and places. These are the same public IDs Discord shows to anyone with
Developer Mode enabled. Migaga does not store usernames, email addresses, IP
addresses or payment information.

### Things you ask Migaga to remember
Some features exist to store something on your behalf. If you use them, that
content is saved:

| Feature | What is stored |
| --- | --- |
| Profiles | Your bio, tag, chosen colour, and any custom profile fields you set |
| Reminders | The reminder text you wrote, when it should fire, and where to send it |
| Points | Point amounts, who sent and received them, and a timestamp |
| Starboard | The ID of the starred message, its author's ID, and the IDs of members who starred it |

### Things your server administrators configure
Server administrators can configure text that Migaga stores against the server,
not against any individual:

- Welcome messages and booster announcement messages
- Custom command names and their responses
- Keyword auto-response rules - the trigger phrase and the reply to send
- Role aliases and role overrides
- Server settings, such as the log channel, command prefix, and points name

### Moderation warnings
If a moderator issues a warning, Migaga stores the warned member's Discord ID,
the server ID, the reason the moderator wrote, and the time it was issued. The
reason text is written by your server's moderators, not by Migaga.

## What Migaga does not store

**Message content is never saved.** Migaga reads messages in order to run keyword
auto-responses and prefix commands, but that content exists only in memory for
the moment it takes to check it. It is never written to the database, never
written to logs, and never sent to any third party.

Server logs are posted to the log channel that your administrators configure.
They live in that channel, inside your own server, and are not copied back to
Migaga.

Migaga does not collect presence data, and does not use the Discord Presence
intent.

## Machine learning and AI

None of the data Migaga stores is used to train machine learning or AI models,
and none of it is sold or shared with advertisers or data brokers.

## Where data is kept and for how long

Data is held in a self-hosted MySQL database. There is no automatic expiry -
data is kept for as long as it is needed to provide the feature it belongs to,
which in practice means for as long as Migaga is in your server.

Removing Migaga from your server stops any further data being recorded, but does
not automatically delete what has already been stored. If you want that data
removed, ask.

## Getting your data deleted

Some data you can remove yourself:

- Profile fields can be unset with the profile commands
- Reminders, custom commands, keyword rules and welcome messages can be deleted
  with their own commands

For anything else - including a full deletion of everything associated with your
Discord account or your server - contact the maintainer:

- On the [Migaga support server](https://server.migaga.info/)

Requests are handled manually, so please allow a reasonable amount of time.

## Changes to this policy

If this policy changes, the date at the top of this page will be updated. Because
the docs site is open source, the full history of changes is visible in the
[repository](https://github.com/LewisHobden/migaga-docs).
