# ActivityPub (activitypub)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

W3C decentralized social networking protocol with a REST API standard for federated social interactions, object delivery, and inbox/outbox management across platforms.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/activitypub/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/activitypub/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Open Standard
- Social Networks
- Federation
- Fediverse
- W3C

## Timestamps

- **Created:** 2026-06-13
- **Modified:** 2026-06-13

## APIs

### ActivityPub Actors API

Actors are the primary objects in ActivityPub that represent entities capable of performing activities. Each actor has a unique IRI and exposes properties such as inbox, outbox, followers, following, and liked collections. Actor objects are retrieved via HTTP GET and served as JSON-LD using the ActivityStreams 2.0 vocabulary.

#### Tags

- Actors
- Profiles
- Social Networks

#### Properties

- [Documentation](https://www.w3.org/TR/activitypub/#actors)
- [API Reference](https://www.w3.org/TR/activitypub/#actor-objects)

### ActivityPub Inbox API

The inbox is an OrderedCollection endpoint on each actor that receives activities delivered by remote servers. Servers POST activities to an actor's inbox to federate content. The inbox also supports GET for authorized clients to retrieve received activities.

#### Tags

- Inbox
- Messages
- Delivery
- Social Networks

#### Properties

- [Documentation](https://www.w3.org/TR/activitypub/#inbox)
- [API Reference](https://www.w3.org/TR/activitypub/#server-to-server-interactions)

### ActivityPub Outbox API

The outbox is an OrderedCollection endpoint that stores activities published by an actor. Clients POST activities to an actor's outbox to create, update, delete, follow, like, and perform other social interactions.

#### Tags

- Outbox
- Publishing
- Activities
- Social Networks

#### Properties

- [Documentation](https://www.w3.org/TR/activitypub/#outbox)
- [API Reference](https://www.w3.org/TR/activitypub/#client-to-server-interactions)

### ActivityPub Followers and Following API

Actors expose followers and following as OrderedCollection or Collection endpoints. These endpoints enumerate the social graph connections for an actor.

#### Tags

- Followers
- Following
- Social Graph
- Social Networks

#### Properties

- [Documentation](https://www.w3.org/TR/activitypub/#followers)
- [API Reference](https://www.w3.org/TR/activitypub/#following)

### ActivityPub Liked Collection API

The liked collection is an optional OrderedCollection endpoint on an actor listing all objects the actor has liked.

#### Tags

- Liked
- Reactions
- Activities
- Social Networks

#### Properties

- [Documentation](https://www.w3.org/TR/activitypub/#liked)

### ActivityPub Object and Activity Delivery API

ActivityPub defines a server-to-server federation protocol for delivering activities between instances. Servers dereference actor inboxes from WebFinger or direct URLs, then HTTP POST signed Activity objects.

#### Tags

- Activities
- Objects
- Delivery
- Federation
- Social Networks

#### Properties

- [Documentation](https://www.w3.org/TR/activitypub/#delivery)
- [API Reference](https://www.w3.org/TR/activitypub/#activity-types)

### ActivityPub WebFinger Discovery API

ActivityPub implementations commonly use WebFinger (RFC 7033) for actor discovery. A GET request to /.well-known/webfinger returns a JSON Resource Descriptor linking to the actor's canonical ActivityPub profile URL.

#### Tags

- WebFinger
- Discovery
- Identity
- Social Networks

#### Properties

- [Documentation](https://www.w3.org/TR/activitypub/#security-considerations)
- [API Reference](https://webfinger.net/)
- [RFC 7033](https://www.rfc-editor.org/rfc/rfc7033)

### ActivityPub NodeInfo API

NodeInfo is a complementary protocol used by ActivityPub servers to expose server capability metadata at /.well-known/nodeinfo.

#### Tags

- NodeInfo
- Discovery
- Server Metadata
- Social Networks

#### Properties

- [Documentation](https://nodeinfo.diaspora.software/)

## Common Properties

- [Website](https://activitypub.rocks/)
- [Specification](https://www.w3.org/TR/activitypub/)
- [Documentation](https://www.w3.org/TR/activitypub/)
- [Getting Started](https://activitypub.rocks/)
- [Authentication](https://www.w3.org/TR/activitypub/#authorization)
- [Security](https://www.w3.org/TR/activitypub/#security-considerations)
- [GitHub Organization](https://github.com/w3c/activitypub)
- [Forum](https://socialhub.activitypub.rocks/)
- [Changelog](https://www.w3.org/TR/activitypub/#change-log)
- [Vocabulary](https://www.w3.org/TR/activitystreams-vocabulary/)
- [Plans](plans/activitypub-plans.yml)
- [Rate Limits](rate-limits/activitypub-rate-limits.yml)
- [FinOps](finops/activitypub-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**FN:** APIs.json
**Email:** info@apis.io
