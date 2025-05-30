# News API

## Sync overview

This source retrieves news stories from the [News API](https://newsapi.org/).
It can retrieve news stories all news stories found within the parameters
chosen, or just top headlines.

### Output schema

This source is capable of syncing the following streams:

- `everything`
- `top_headlines`

### Features

| Feature           | Supported? \(Yes/No\) | Notes |
| :---------------- | :-------------------- | :---- |
| Full Refresh Sync | Yes                   |       |
| Incremental Sync  | No                    |       |

### Performance considerations

The News API free tier only allows 100 requests per day, and only up to 100
results per request. It is not recommended to attempt to use this source with
a free tier API key.

## Getting started

### Requirements

1. A News API key. You can get one [here](https://newsapi.org/). It is
   highly recommended to use a paid tier key.

### Setup guide

The following fields are required fields for the connector to work:

- `api_key`: Your News API key.
- (optional) `search_query`: A search query to filter the results by. For more
  information on constructing a search query, see the
  [News API documentation](https://newsapi.org/docs/endpoints/everything).
- (optional) `search_in`: Fields to search in. Possible values are `title`,
  `description` and `content`.
- (optional) `sources`: Sources to search in. For a list of sources, see the
  [News API documentation](https://newsapi.org/sources).
- (optional) `domains`: Domains to search in.
- (optional) `exclude_domains`: Domains to exclude from the search.
- (optional) `start_date`: The start date to search from.
- (optional) `end_date`: The end date to search to.
- (optional) `language`: The language to search in.
- `country`: The country you want headlines for.
- `category`: The category you want headlines for.
- `sort_by`: How to sort the results.

## Changelog

<details>
  <summary>Expand to review</summary>

| Version | Date       | Pull Request                                             | Subject                                  |
|:--------|:-----------| :------------------------------------------------------- | :--------------------------------------- |
| 0.2.23 | 2025-05-24 | [60578](https://github.com/airbytehq/airbyte/pull/60578) | Update dependencies |
| 0.2.22 | 2025-05-10 | [59468](https://github.com/airbytehq/airbyte/pull/59468) | Update dependencies |
| 0.2.21 | 2025-04-27 | [58520](https://github.com/airbytehq/airbyte/pull/58520) | Update dependencies |
| 0.2.20 | 2025-04-12 | [57848](https://github.com/airbytehq/airbyte/pull/57848) | Update dependencies |
| 0.2.19 | 2025-04-05 | [57286](https://github.com/airbytehq/airbyte/pull/57286) | Update dependencies |
| 0.2.18 | 2025-03-29 | [56690](https://github.com/airbytehq/airbyte/pull/56690) | Update dependencies |
| 0.2.17 | 2025-03-22 | [56009](https://github.com/airbytehq/airbyte/pull/56009) | Update dependencies |
| 0.2.16 | 2025-03-08 | [55451](https://github.com/airbytehq/airbyte/pull/55451) | Update dependencies |
| 0.2.15 | 2025-03-01 | [54812](https://github.com/airbytehq/airbyte/pull/54812) | Update dependencies |
| 0.2.14 | 2025-02-22 | [54325](https://github.com/airbytehq/airbyte/pull/54325) | Update dependencies |
| 0.2.13 | 2025-02-15 | [53850](https://github.com/airbytehq/airbyte/pull/53850) | Update dependencies |
| 0.2.12 | 2025-02-08 | [53275](https://github.com/airbytehq/airbyte/pull/53275) | Update dependencies |
| 0.2.11 | 2025-02-01 | [52714](https://github.com/airbytehq/airbyte/pull/52714) | Update dependencies |
| 0.2.10 | 2025-01-25 | [52272](https://github.com/airbytehq/airbyte/pull/52272) | Update dependencies |
| 0.2.9 | 2025-01-18 | [51783](https://github.com/airbytehq/airbyte/pull/51783) | Update dependencies |
| 0.2.8 | 2025-01-11 | [51222](https://github.com/airbytehq/airbyte/pull/51222) | Update dependencies |
| 0.2.7 | 2024-12-28 | [50602](https://github.com/airbytehq/airbyte/pull/50602) | Update dependencies |
| 0.2.6 | 2024-12-21 | [50071](https://github.com/airbytehq/airbyte/pull/50071) | Update dependencies |
| 0.2.5 | 2024-12-14 | [49214](https://github.com/airbytehq/airbyte/pull/49214) | Update dependencies |
| 0.2.4 | 2024-11-04 | [48143](https://github.com/airbytehq/airbyte/pull/48143) | Update dependencies |
| 0.2.3 | 2024-10-29 | [47866](https://github.com/airbytehq/airbyte/pull/47866) | Update dependencies |
| 0.2.2 | 2024-10-28 | [47562](https://github.com/airbytehq/airbyte/pull/47562) | Update dependencies |
| 0.2.1 | 2024-08-16 | [44196](https://github.com/airbytehq/airbyte/pull/44196) | Bump source-declarative-manifest version |
| 0.2.0 | 2024-08-15 | [44114](https://github.com/airbytehq/airbyte/pull/44114) | Refactor connector to manifest-only format |
| 0.1.15 | 2024-08-12 | [43908](https://github.com/airbytehq/airbyte/pull/43908) | Update dependencies |
| 0.1.14 | 2024-08-10 | [43589](https://github.com/airbytehq/airbyte/pull/43589) | Update dependencies |
| 0.1.13 | 2024-08-03 | [43096](https://github.com/airbytehq/airbyte/pull/43096) | Update dependencies |
| 0.1.12 | 2024-07-27 | [42820](https://github.com/airbytehq/airbyte/pull/42820) | Update dependencies |
| 0.1.11 | 2024-07-20 | [42285](https://github.com/airbytehq/airbyte/pull/42285) | Update dependencies |
| 0.1.10 | 2024-07-13 | [41781](https://github.com/airbytehq/airbyte/pull/41781) | Update dependencies |
| 0.1.9 | 2024-07-10 | [41599](https://github.com/airbytehq/airbyte/pull/41599) | Update dependencies |
| 0.1.8 | 2024-07-09 | [41200](https://github.com/airbytehq/airbyte/pull/41200) | Update dependencies |
| 0.1.7 | 2024-07-06 | [40802](https://github.com/airbytehq/airbyte/pull/40802) | Update dependencies |
| 0.1.6 | 2024-06-25 | [40297](https://github.com/airbytehq/airbyte/pull/40297) | Update dependencies |
| 0.1.5 | 2024-06-22 | [40174](https://github.com/airbytehq/airbyte/pull/40174) | Update dependencies |
| 0.1.4 | 2024-06-12 | [38635](https://github.com/airbytehq/airbyte/pull/38635) | Use Poetry, remove $parameters, make Builder compatible |
| 0.1.3 | 2024-06-04 | [39038](https://github.com/airbytehq/airbyte/pull/39038) | [autopull] Upgrade base image to v1.2.1 |
| 0.1.2 | 2024-05-20 | [38418](https://github.com/airbytehq/airbyte/pull/38418) | [autopull] base image + poetry + up_to_date |
| 0.1.1 | 2023-04-30 | [25554](https://github.com/airbytehq/airbyte/pull/25554) | Make manifest connector builder friendly |
| 0.1.0 | 2022-10-21 | [18301](https://github.com/airbytehq/airbyte/pull/18301) | New source |

</details>
