# MB
**MetaBrani** berdiri untuk **Metode Ekonomi Tinggi Atas Bawah Rendah Awal Nilai Inti**.
Mereka ada untuk mendokumentasikan apa yang mungkin dilaksanakan oleh [BejoFx](https://evositas.github.io) dan [FxBejo](x.com/metabrani)
`Halaman masih dalam renovasi`

---

- [Daftar](#daftar)
- [Jenis Acara](#jenis-acara)
  - [Rentang Jenis Acara](#rentang-jenis-acara)
- [Jenis Pesan](#jenis-pesan)
  - [Daftar Akun](#daftar-akun)
  - [Perkiraan Harga](#perkiraan-harga)
- [Peringatan Risiko](#peringatan-risiko)
- [Halaman masih dalam renovasi](#halaman-masih-dalam-renovasi)
- [License](#license)

---

### Relay to Client

| type     | description                                             | Sebaran     |
| -------- | ------------------------------------------------------- | ----------- |
| `EURUSD` | Pasangan mata uang EUR dan USD, EROPA-Amerika Serikat   | [01](01.md) |
| `BTCUSD` | Pasangan Bitcoin dan USD, Dunia-Amerika Serikat         | [1600](01.md) |
| `XAUUSD` | Pasangan mata uang Emas dan USD, Dunia-Amerika Serikat  | [36](01.md) |
| `USDCHF` | Pasangan mata uang USD dan CHF, AS-Swiss                | [01](01.md) |
| `GBPUSD` | Pasangan mata uang GPB dan USD, Inggris-AS              | [03](42.md) |
| `USDJPY` | Pasangan mata uang USD dan JPY, AS-Jepang               | [04](45.md) |

Akan diperbarui jika ada hal yang akan diperbarui.

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

