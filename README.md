# MB
METABRANI stand for **Metode Ekonomi Tinggi Atas Bawah Rendah Awal Nilai Inti**.
Mereka ada untuk mendokumentasikan apa yang mungkin dilaksanakan oleh [Evositas](https://evositas.github.io)

---

- [List](#list)
- [Event Kinds](#event-kinds)
  - [Event Kind Ranges](#event-kind-ranges)
- [Message Types](#message-types)
  - [Client to Relay](#client-to-relay)
  - [Relay to Client](#relay-to-client)
- [Standardized Tags](#standardized-tags)
- [Criteria for acceptance of NIPs](#criteria-for-acceptance-of-nips)
- [License](#license)

---

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

