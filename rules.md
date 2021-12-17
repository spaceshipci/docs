# SpaceshipCI usage Rules

In order to get a good service, we create rules for the User of SpachipCi as explained bellow:
- One login ID SHOULD NOT used by multiple person
- One login ID SHOULD NOT queued a job right bellow their currently running job. At least there is one job of other users then you can queue your new job
- One login ID SHOULD NOT have more than 5 jobs.
- User SHOULD NOT run multiple task in one job. Example: Adding downlaoding ROM Source, then directly build the ROM at the same time. Or, doing a build for multiple devices. But, building kernel for max 5 devices is allowed.
- User SHOULD NOT abort other user's job or job queue
- User SHOULD NOT Download ROM Source from SSH. It's allowed if there is exception from the admin for Downloading Private ROM source.
- User SHOULD NOT read or even modify other user's home directory and jenkins job


Violation of the rules will be penalized by being suspended from the server
