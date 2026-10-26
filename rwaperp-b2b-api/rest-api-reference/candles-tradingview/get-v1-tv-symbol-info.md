# get v1 tv symbol info

`GET /v1/tv/symbol_info`

**Authentication:** None

**Rate limit:** 10 requests per 1 second per IP address

## Parameters

| Name    | Location | Type   | Required | Description |
| ------- | -------- | ------ | -------- | ----------- |
| `group` | query    | string | Yes      | —           |

## Responses

### HTTP 200

OK

| Field                    | Type          | Required | Description |
| ------------------------ | ------------- | -------- | ----------- |
| `s`                      | string        | Yes      | —           |
| `symbol`                 | array         | Yes      | —           |
| `description`            | array         | Yes      | —           |
| `currency`               | array         | Yes      | —           |
| `base-currency`          | array         | Yes      | —           |
| `exchange-listed`        | array         | Yes      | —           |
| `exchange-traded`        | array         | Yes      | —           |
| `minmovement`            | array         | Yes      | —           |
| `minmovement2`           | array         | Yes      | —           |
| `fractional`             | array         | Yes      | —           |
| `pricescale`             | array         | Yes      | —           |
| `root`                   | array         | Yes      | —           |
| `root-description`       | array         | Yes      | —           |
| `has-intraday`           | array         | Yes      | —           |
| `has-no-volume`          | array         | Yes      | —           |
| `type`                   | array         | Yes      | —           |
| `is-cfd`                 | array         | Yes      | —           |
| `ticker`                 | array         | Yes      | —           |
| `timezone`               | array         | Yes      | —           |
| `session-regular`        | array         | Yes      | —           |
| `session-extended`       | array         | Yes      | —           |
| `session-premarket`      | array         | Yes      | —           |
| `session-postmarket`     | array         | Yes      | —           |
| `supported-resolutions`  | array\<array> | Yes      | —           |
| `has-daily`              | array         | Yes      | —           |
| `intraday-multipliers`   | array\<array> | Yes      | —           |
| `has-weekly-and-monthly` | array         | Yes      | —           |
| `pointvalue`             | array         | Yes      | —           |
| `expiration`             | array         | Yes      | —           |
| `bar-source`             | array         | Yes      | —           |
| `bar-transform`          | array         | Yes      | —           |
| `bar-fillgaps`           | array         | Yes      | —           |
| `isin`                   | array         | Yes      | —           |
| `wkn`                    | array         | Yes      | —           |
