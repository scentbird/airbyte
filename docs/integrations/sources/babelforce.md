# Babelforce

## Overview

The Babelforce source supports _Full Refresh_ as well as _Incremental_ syncs.

_Full Refresh_ sync means every time a sync is run, Airbyte will copy all rows in the tables and columns you set up for replication into the destination in a new table.
_Incremental_ syn means only changed resources are copied from Babelformce. For the first run, it will be a Full Refresh sync.

### Output schema

Several output streams are available from this source:

- [Calls](https://api.babelforce.com/#af7a6b6e-b262-487f-aabd-c59e6fe7ba41)

If there are more endpoints you'd like Airbyte to support, please [create an issue.](https://github.com/airbytehq/airbyte/issues/new/choose)

### Features

| Feature                       | Supported?  |
| :---------------------------- | :---------- |
| Full Refresh Sync             | Yes         |
| Incremental Sync              | Yes         |
| Replicate Incremental Deletes | Coming soon |
| SSL connection                | Yes         |
| Namespaces                    | No          |

### Performance considerations

There are no performance consideration in the current version.

## Getting started

### Requirements

- Region/environment as listed in the `Regions & environments` section [here](https://api.babelforce.com/#intro)
- Babelforce access key ID
- Babelforce access token
- (Optional) start date from when the import starts in epoch Unix timestamp

### Setup guide

Generate a API access key ID and token using the [Babelforce documentation](https://help.babelforce.com/hc/en-us/articles/360044753932-API-documentation-and-endpoints-an-introduction-)

## Changelog

<details>
  <summary>Expand to review</summary>

| Version | Date       | Pull Request                                             | Subject                     |
| :------ | :--------- | :------------------------------------------------------- | :-------------------------- |
| 0.3.25 | 2025-05-17 | [60625](https://github.com/airbytehq/airbyte/pull/60625) | Update dependencies |
| 0.3.24 | 2025-05-10 | [59821](https://github.com/airbytehq/airbyte/pull/59821) | Update dependencies |
| 0.3.23 | 2025-05-03 | [59346](https://github.com/airbytehq/airbyte/pull/59346) | Update dependencies |
| 0.3.22 | 2025-04-26 | [58686](https://github.com/airbytehq/airbyte/pull/58686) | Update dependencies |
| 0.3.21 | 2025-04-19 | [58239](https://github.com/airbytehq/airbyte/pull/58239) | Update dependencies |
| 0.3.20 | 2025-04-12 | [57613](https://github.com/airbytehq/airbyte/pull/57613) | Update dependencies |
| 0.3.19 | 2025-04-05 | [57182](https://github.com/airbytehq/airbyte/pull/57182) | Update dependencies |
| 0.3.18 | 2025-03-29 | [56595](https://github.com/airbytehq/airbyte/pull/56595) | Update dependencies |
| 0.3.17 | 2025-03-22 | [56110](https://github.com/airbytehq/airbyte/pull/56110) | Update dependencies |
| 0.3.16 | 2025-03-08 | [55392](https://github.com/airbytehq/airbyte/pull/55392) | Update dependencies |
| 0.3.15 | 2025-03-01 | [54838](https://github.com/airbytehq/airbyte/pull/54838) | Update dependencies |
| 0.3.14 | 2025-02-22 | [54219](https://github.com/airbytehq/airbyte/pull/54219) | Update dependencies |
| 0.3.13 | 2025-02-15 | [53912](https://github.com/airbytehq/airbyte/pull/53912) | Update dependencies |
| 0.3.12 | 2025-02-08 | [53392](https://github.com/airbytehq/airbyte/pull/53392) | Update dependencies |
| 0.3.11 | 2025-02-01 | [52919](https://github.com/airbytehq/airbyte/pull/52919) | Update dependencies |
| 0.3.10 | 2025-01-25 | [52182](https://github.com/airbytehq/airbyte/pull/52182) | Update dependencies |
| 0.3.9 | 2025-01-18 | [51776](https://github.com/airbytehq/airbyte/pull/51776) | Update dependencies |
| 0.3.8 | 2025-01-11 | [51275](https://github.com/airbytehq/airbyte/pull/51275) | Update dependencies |
| 0.3.7 | 2024-12-28 | [50502](https://github.com/airbytehq/airbyte/pull/50502) | Update dependencies |
| 0.3.6 | 2024-12-21 | [50184](https://github.com/airbytehq/airbyte/pull/50184) | Update dependencies |
| 0.3.5 | 2024-12-14 | [49587](https://github.com/airbytehq/airbyte/pull/49587) | Update dependencies |
| 0.3.4 | 2024-12-12 | [49286](https://github.com/airbytehq/airbyte/pull/49286) | Update dependencies |
| 0.3.3 | 2024-12-11 | [49035](https://github.com/airbytehq/airbyte/pull/49035) | Starting with this version, the Docker image is now rootless. Please note that this and future versions will not be compatible with Airbyte versions earlier than 0.64 |
| 0.3.2 | 2024-10-28 | [47631](https://github.com/airbytehq/airbyte/pull/47631) | Update dependencies |
| 0.3.1 | 2024-08-16 | [44196](https://github.com/airbytehq/airbyte/pull/44196) | Bump source-declarative-manifest version |
| 0.3.0 | 2024-08-09 | [43439](https://github.com/airbytehq/airbyte/pull/43439) | Refactor connector to manifest-only format |
| 0.2.12 | 2024-08-03 | [43191](https://github.com/airbytehq/airbyte/pull/43191) | Update dependencies |
| 0.2.11 | 2024-07-27 | [42633](https://github.com/airbytehq/airbyte/pull/42633) | Update dependencies |
| 0.2.10 | 2024-07-20 | [42239](https://github.com/airbytehq/airbyte/pull/42239) | Update dependencies |
| 0.2.9 | 2024-07-13 | [41728](https://github.com/airbytehq/airbyte/pull/41728) | Update dependencies |
| 0.2.8 | 2024-07-10 | [41508](https://github.com/airbytehq/airbyte/pull/41508) | Update dependencies |
| 0.2.7 | 2024-07-09 | [41260](https://github.com/airbytehq/airbyte/pull/41260) | Update dependencies |
| 0.2.6 | 2024-07-06 | [40911](https://github.com/airbytehq/airbyte/pull/40911) | Update dependencies |
| 0.2.5 | 2024-06-25 | [40386](https://github.com/airbytehq/airbyte/pull/40386) | Update dependencies |
| 0.2.4 | 2024-06-22 | [39963](https://github.com/airbytehq/airbyte/pull/39963) | Update dependencies |
| 0.2.3 | 2024-06-12 | [38776](https://github.com/airbytehq/airbyte/pull/38776) | Make connector compatible with Builder |
| 0.2.2 | 2024-06-06 | [39163](https://github.com/airbytehq/airbyte/pull/39163) | [autopull] Upgrade base image to v1.2.2 |
| 0.2.1 | 2024-05-21 | [38523](https://github.com/airbytehq/airbyte/pull/38523) | [autopull] base image + poetry + up_to_date |
| 0.2.0 | 2023-08-24 | [29314](https://github.com/airbytehq/airbyte/pull/29314) | Migrate to Low Code |
| 0.1.0 | 2022-05-09 | [12700](https://github.com/airbytehq/airbyte/pull/12700) | Introduce Babelforce source |

</details>
