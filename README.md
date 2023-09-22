# metabrani - Metode Ekonomi Tinggi Atas Bawah Rendah Awal Nilai Inti

MetaBrani berdiri untuk **Metode Ekonomi Tinggi Atas Bawah Rendah Awal Nilai Inti**.
Mereka ada untuk mendokumentasikan apa yang mungkin dilaksanakan oleh [evositas](https://evositas.github.io)

---

- [Daftar](#daftar)
- [Jenis Acara](#jenis-acara)
  - [Rentang Jenis Acara](#event-kind-ranges)

---

## List





## Event Kinds

| kind    | description                | NIP         |
| ------- | -------------------------- | ----------- |
| `0`     | Metadata                   | [1](01.md)  |
| `1`     | Short Text Note            | [1](01.md)  |
| `2`     | Recommend Relay            |             |
| `3`     | Contacts                   | [2](02.md)  |
| `4`     | Encrypted Direct Messages  | [4](04.md)  |
| `5`     | Event Deletion             | [9](09.md)  |
| `6`     | Repost                     | [18](18.md) |
| `7`     | Reaction                   | [25](25.md) |
| `8`     | Badge Award                | [58](58.md) |
| `16`    | Generic Repost             | [18](18.md) |
| `40`    | Channel Creation           | [28](28.md) |
| `41`    | Channel Metadata           | [28](28.md) |
| `42`    | Channel Message            | [28](28.md) |
| `43`    | Channel Hide Message       | [28](28.md) |
| `44`    | Channel Mute User          | [28](28.md) |
| `1063`  | File Metadata              | [94](94.md) |
| `1311`  | Live Chat Message          | [53](53.md) |
| `1984`  | Reporting                  | [56](56.md) |
| `1985`  | Label                      | [32](32.md) |
| `4550`  | Community Post Approval    | [72](72.md) |
| `9041`  | Zap Goal                   | [75](75.md) |
| `9734`  | Zap Request                | [57](57.md) |
| `9735`  | Zap                        | [57](57.md) |
| `10000` | Mute List                  | [51](51.md) |
| `10001` | Pin List                   | [51](51.md) |
| `10002` | Relay List Metadata        | [65](65.md) |
| `13194` | Wallet Info                | [47](47.md) |
| `22242` | Client Authentication      | [42](42.md) |
| `23194` | Wallet Request             | [47](47.md) |
| `23195` | Wallet Response            | [47](47.md) |
| `24133` | Nostr Connect              | [46](46.md) |
| `27235` | HTTP Auth                  | [98](98.md) |
| `30000` | Categorized People List    | [51](51.md) |
| `30001` | Categorized Bookmark List  | [51](51.md) |
| `30008` | Profile Badges             | [58](58.md) |
| `30009` | Badge Definition           | [58](58.md) |
| `30017` | Create or update a stall   | [15](15.md) |
| `30018` | Create or update a product | [15](15.md) |
| `30023` | Long-form Content          | [23](23.md) |
| `30024` | Draft Long-form Content    | [23](23.md) |
| `30078` | Application-specific Data  | [78](78.md) |
| `30311` | Live Event                 | [53](53.md) |
| `30315` | User Statuses              | [38](38.md) |
| `30402` | Classified Listing         | [99](99.md) |
| `30403` | Draft Classified Listing   | [99](99.md) |
| `31922` | Date-Based Calendar Event  | [52](52.md) |
| `31923` | Time-Based Calendar Event  | [52](52.md) |
| `31924` | Calendar                   | [52](52.md) |
| `31925` | Calendar Event RSVP        | [52](52.md) |
| `31989` | Handler recommendation     | [89](89.md) |
| `31990` | Handler information        | [89](89.md) |
| `34550` | Community Definition       | [72](72.md) |


## Message types

### Client to Relay

| type    | description                                         | NIP         |
| ------- | --------------------------------------------------- | ----------- |
| `EVENT` | used to publish events                              | [01](01.md) |
| `REQ`   | used to request events and subscribe to new updates | [01](01.md) |
| `CLOSE` | used to stop previous subscriptions                 | [01](01.md) |
| `AUTH`  | used to send authentication events                  | [42](42.md) |
| `COUNT` | used to request event counts                        | [45](45.md) |

### Relay to Client

| type     | description                                             | NIP         |
| -------- | ------------------------------------------------------- | ----------- |
| `EOSE`   | used to notify clients all stored events have been sent | [01](01.md) |
| `EVENT`  | used to send events requested to clients                | [01](01.md) |
| `NOTICE` | used to send human-readable messages to clients         | [01](01.md) |
| `OK`     | used to notify clients if an EVENT was successful       | [01](01.md) |
| `AUTH`   | used to send authentication challenges                  | [42](42.md) |
| `COUNT`  | used to send requested event counts to clients          | [45](45.md) |

Please update these lists when proposing NIPs introducing new event kinds.

## Standardized Tags

| name              | value                                | other parameters     | NIP                      |
| ----------------- | ------------------------------------ | -------------------- | ------------------------ |
| `e`               | event id (hex)                       | relay URL, marker    | [01](01.md), [10](10.md) |
| `p`               | pubkey (hex)                         | relay URL, petname   | [01](01.md), [02](02.md) |
| `a`               | coordinates to an event              | relay URL            | [01](01.md)              |
| `d`               | identifier                           | --                   | [01](01.md)              |
| `alt`             | summary                              | --                   | [31](31.md)              |
| `g`               | geohash                              | --                   | [52](52.md)              |
| `i`               | identity                             | proof                | [39](39.md)              |
| `k`               | kind number (string)                 | --                   | [18](18.md), [72](72.md) |
| `l`               | label, label namespace               | annotations          | [32](32.md)              |
| `L`               | label namespace                      | --                   | [32](32.md)              |
| `m`               | MIME type                            | --                   | [94](94.md)              |
| `r`               | a reference (URL, etc)               | petname              |                          |
| `r`               | relay url                            | marker               | [65](65.md)              |
| `t`               | hashtag                              | --                   |                          |
| `amount`          | millisatoshis, stringified           | --                   | [57](57.md)              |
| `bolt11`          | `bolt11` invoice                     | --                   | [57](57.md)              |
| `challenge`       | challenge string                     | --                   | [42](42.md)              |
| `content-warning` | reason                               | --                   | [36](36.md)              |
| `delegation`      | pubkey, conditions, delegation token | --                   | [26](26.md)              |
| `description`     | invoice/badge description            | --                   | [57](57.md), [58](58.md) |
| `emoji`           | shortcode, image URL                 | --                   | [30](30.md)              |
| `expiration`      | unix timestamp (string)              | --                   | [40](40.md)              |
| `goal`            | event id (hex)                       | relay URL            | [75](75.md)              |
| `image`           | image URL                            | dimensions in pixels | [23](23.md), [58](58.md) |
| `lnurl`           | `bech32` encoded `lnurl`             | --                   | [57](57.md)              |
| `location`        | location string                      | --                   | [52](52.md), [99](99.md) |
| `name`            | badge name                           | --                   | [58](58.md)              |
| `nonce`           | random                               | --                   | [13](13.md)              |
| `preimage`        | hash of `bolt11` invoice             | --                   | [57](57.md)              |
| `price`           | price                                | currency, frequency  | [99](99.md)              |
| `proxy`           | external ID                          | protocol             | [48](48.md)              |
| `published_at`    | unix timestamp (string)              | --                   | [23](23.md)              |
| `relay`           | relay url                            | --                   | [42](42.md)              |
| `relays`          | relay list                           | --                   | [57](57.md)              |
| `subject`         | subject                              | --                   | [14](14.md)              |
| `summary`         | article summary                      | --                   | [23](23.md)              |
| `thumb`           | badge thumbnail                      | dimensions in pixels | [58](58.md)              |
| `title`           | article title                        | --                   | [23](23.md)              |
| `zap`             | pubkey (hex), relay URL              | weight               | [57](57.md)              |

## Criteria for acceptance of NIPs

1. They should be implemented in at least two clients and one relay -- when applicable.
2. They should make sense.
3. They should be optional and backwards-compatible: care must be taken such that clients and relays that choose to not implement them do not stop working when interacting with the ones that choose to.
4. There should be no more than one way of doing the same thing.
5. Other rules will be made up when necessary.

## Mailing Lists


## License
