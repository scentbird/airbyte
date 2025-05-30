# K6 Cloud API

## Sync overview

This source can sync data from the [K6 Cloud API](https://developers.k6.io). At present this connector only supports full refresh syncs meaning that each time you use the connector it will sync all available records from scratch. Please use cautiously if you expect your API to have a lot of records.

## This Source Supports the Following Streams

- organizations
- projects
- tests

### Features

| Feature           | Supported?\(Yes/No\) | Notes |
| :---------------- | :------------------- | :---- |
| Full Refresh Sync | Yes                  |       |
| Incremental Sync  | No                   |       |

### Performance considerations

## Getting started

### Requirements

- API Token

## Changelog

<details>
  <summary>Expand to review</summary>

| Version | Date       | Pull Request                                              | Subject                                                                         |
| :------ | :--------- | :-------------------------------------------------------- | :------------------------------------------------------------------------------ |
| 0.2.26 | 2025-05-24 | [60713](https://github.com/airbytehq/airbyte/pull/60713) | Update dependencies |
| 0.2.25 | 2025-05-10 | [59830](https://github.com/airbytehq/airbyte/pull/59830) | Update dependencies |
| 0.2.24 | 2025-05-03 | [59232](https://github.com/airbytehq/airbyte/pull/59232) | Update dependencies |
| 0.2.23 | 2025-04-26 | [58780](https://github.com/airbytehq/airbyte/pull/58780) | Update dependencies |
| 0.2.22 | 2025-04-19 | [58224](https://github.com/airbytehq/airbyte/pull/58224) | Update dependencies |
| 0.2.21 | 2025-04-12 | [57693](https://github.com/airbytehq/airbyte/pull/57693) | Update dependencies |
| 0.2.20 | 2025-04-05 | [57092](https://github.com/airbytehq/airbyte/pull/57092) | Update dependencies |
| 0.2.19 | 2025-03-29 | [56698](https://github.com/airbytehq/airbyte/pull/56698) | Update dependencies |
| 0.2.18 | 2025-03-22 | [56019](https://github.com/airbytehq/airbyte/pull/56019) | Update dependencies |
| 0.2.17 | 2025-03-08 | [55486](https://github.com/airbytehq/airbyte/pull/55486) | Update dependencies |
| 0.2.16 | 2025-03-01 | [54748](https://github.com/airbytehq/airbyte/pull/54748) | Update dependencies |
| 0.2.15 | 2025-02-22 | [54290](https://github.com/airbytehq/airbyte/pull/54290) | Update dependencies |
| 0.2.14 | 2025-02-15 | [53830](https://github.com/airbytehq/airbyte/pull/53830) | Update dependencies |
| 0.2.13 | 2025-02-08 | [53251](https://github.com/airbytehq/airbyte/pull/53251) | Update dependencies |
| 0.2.12 | 2025-02-01 | [52732](https://github.com/airbytehq/airbyte/pull/52732) | Update dependencies |
| 0.2.11 | 2025-01-25 | [52229](https://github.com/airbytehq/airbyte/pull/52229) | Update dependencies |
| 0.2.10 | 2025-01-18 | [51837](https://github.com/airbytehq/airbyte/pull/51837) | Update dependencies |
| 0.2.9 | 2025-01-11 | [51190](https://github.com/airbytehq/airbyte/pull/51190) | Update dependencies |
| 0.2.8 | 2024-12-28 | [50656](https://github.com/airbytehq/airbyte/pull/50656) | Update dependencies |
| 0.2.7 | 2024-12-21 | [50077](https://github.com/airbytehq/airbyte/pull/50077) | Update dependencies |
| 0.2.6 | 2024-12-14 | [49612](https://github.com/airbytehq/airbyte/pull/49612) | Update dependencies |
| 0.2.5 | 2024-12-12 | [49242](https://github.com/airbytehq/airbyte/pull/49242) | Update dependencies |
| 0.2.4 | 2024-12-11 | [48204](https://github.com/airbytehq/airbyte/pull/48204) | Starting with this version, the Docker image is now rootless. Please note that this and future versions will not be compatible with Airbyte versions earlier than 0.64 |
| 0.2.3 | 2024-10-29 | [47895](https://github.com/airbytehq/airbyte/pull/47895) | Update dependencies |
| 0.2.2 | 2024-10-28 | [47454](https://github.com/airbytehq/airbyte/pull/47454) | Update dependencies |
| 0.2.1 | 2024-08-16 | [44196](https://github.com/airbytehq/airbyte/pull/44196) | Bump source-declarative-manifest version |
| 0.2.0 | 2024-08-15 | [44137](https://github.com/airbytehq/airbyte/pull/44137) | Refactor connector to manifest-only format |
| 0.1.15 | 2024-08-10 | [43493](https://github.com/airbytehq/airbyte/pull/43493) | Update dependencies |
| 0.1.14 | 2024-08-03 | [43077](https://github.com/airbytehq/airbyte/pull/43077) | Update dependencies |
| 0.1.13 | 2024-07-27 | [42789](https://github.com/airbytehq/airbyte/pull/42789) | Update dependencies |
| 0.1.12 | 2024-07-20 | [42249](https://github.com/airbytehq/airbyte/pull/42249) | Update dependencies |
| 0.1.11 | 2024-07-13 | [41871](https://github.com/airbytehq/airbyte/pull/41871) | Update dependencies |
| 0.1.10 | 2024-07-10 | [41462](https://github.com/airbytehq/airbyte/pull/41462) | Update dependencies |
| 0.1.9 | 2024-07-10 | [41324](https://github.com/airbytehq/airbyte/pull/41324) | Update dependencies |
| 0.1.8 | 2024-07-06 | [40875](https://github.com/airbytehq/airbyte/pull/40875) | Update dependencies |
| 0.1.7 | 2024-06-25 | [40291](https://github.com/airbytehq/airbyte/pull/40291) | Update dependencies |
| 0.1.6 | 2024-06-21 | [39921](https://github.com/airbytehq/airbyte/pull/39921) | Update dependencies |
| 0.1.5 | 2024-06-04 | [39044](https://github.com/airbytehq/airbyte/pull/39044) | [autopull] Upgrade base image to v1.2.1 |
| 0.1.4 | 2024-05-15 | [38150](https://github.com/airbytehq/airbyte/pull/38150) | Make connector compatable with the builder |
| 0.1.3 | 2024-04-19 | [37181](https://github.com/airbytehq/airbyte/pull/37181) | Upgrade to CDK 0.80.0 and manage dependencies with Poetry. |
| 0.1.2 | 2024-04-15 | [37181](https://github.com/airbytehq/airbyte/pull/37181) | Base image migration: remove Dockerfile and use the python-connector-base image |
| 0.1.1 | 2024-04-12 | [37181](https://github.com/airbytehq/airbyte/pull/37181) | schema descriptions |
| 0.1.0   | 2022-10-27 | [#18393](https://github.com/airbytehq/airbyte/pull/18393) | 🎉 New Source: K6 Cloud API [low-code CDK]                                      |

</details>
