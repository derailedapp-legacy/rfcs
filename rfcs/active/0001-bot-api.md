# Bot API
Bot's are an essential part of every chat platform. One of the biggest reasons Discord is loved so much is because of it's vast, easy, 
and expansive Bot API along with many tools to help you learn.

Derailed will be implementing bots/applications itself. Integrally, we want this API to be as easy to use as possible and be as open as possible.
Any part of Derailed's API which can be used by bots, will be.

Discord themselves locks off features to big applications stating unexistent "safety" reasons.
Derailed will be giving you a grip on your fullest potential, we won't be **ever** locking out our API to big applications.

But anyway, with that done, let's get onto the actual design part!

## Possible Application Object

| field   | type      |
| ------- | --------- |
| id      | snowflake |
| name    | string    |
| owner   | snowflake |
| has_bot | boolean   |

An "Application" is a superset of a bot. Bot's are applications but it could not be vice versa.

Applications have access to what will in the future become our oauth2 suite, 
bot's are just users with some missing features and are supposed to be for automation.

Think: Applications can be used as a login for your merch storefront, but Bot's can be used intertwined for your storefronts sales announcements.

That's the difference and similarity.

## What else?
Nothing else really, bot's lose access to some features like readstates since they don't need it, 
and a new field to the user object is added. "Bot."

Bot's will have full access to our voice & video suite, allowing them to: talk, listen, stream, and share their cameras.
Basically, bot's are automated users. That's it.
