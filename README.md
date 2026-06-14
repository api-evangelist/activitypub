# ActivityPub (activitypub)

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
