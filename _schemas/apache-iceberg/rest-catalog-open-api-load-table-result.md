---
description: 'Result used when a table is successfully loaded. The table metadata JSON is returned in the `metadata` field. The corresponding file location of table metadata should be returned in the `metadata-location` field, unless the metadata is not yet committed. For example, a create transaction may return metadata that is staged but not committed. Clients can check whether metadata has changed by comparing metadata locations after the table has been created. The `config` map returns table-specific configuration for the table''s resources, including its HTTP client and FileIO. For example, config may contain a specific FileIO implementation class for the table depending on its underlying storage. The following configurations should be respected by clients: ## General Configurations - `token`: Authorization bearer token to use for table requests if OAuth2 security is enabled - `scan-planning-mode`: Communicates to clients the supported planning mode. Clients should use this value to
  fail fast if the supported scanning mode is not available on the client. Valid values: - `client`: Clients MUST use client-side scan planning - `server`: Clients MUST use server-side scan planning via the `planTableScan` endpoint ## AWS Configurations The following configurations should be respected when working with tables stored in AWS S3 - `client.region`: region to configure client for making requests to AWS - `s3.access-key-id`: id for credentials that provide access to the data in S3 - `s3.secret-access-key`: secret for credentials that provide access to data in S3 - `s3.session-token`: if present, this value should be used for as the session token - `s3.remote-signing-enabled`: if `true` remote signing should be performed as described in the `RemoteSignRequest` schema section of this spec document. - `s3.cross-region-access-enabled`: if `true`, S3 Cross-Region bucket access is enabled ## Storage Credentials Credentials for ADLS / GCS / S3 / ... are provided through the `storage-credentials`
  field. Clients must first check whether the respective credentials exist in the `storage-credentials` field before checking the `config` for credentials. ## Remote Signing If remote signing for a specific storage provider is enabled, clients must respect the following configurations when creating a remote signer client: - `signer.endpoint`: the remote signer endpoint. Required. Can either be a relative path (to be resolved against `signer.uri`) or an absolute URI. - `signer.uri`: the base URI to resolve `signer.endpoint` against. Optional. Only meaningful if `signer.endpoint` is a relative path. Defaults to the catalog''s base URI if not set.'
layout: schema
name: LoadTableResult
properties_list:
- description: May be null if the table is staged as part of a transaction
  name: metadata-location
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: config
  type: object
- description: ''
  name: storage-credentials
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-load-table-result-schema.json
slug: rest-catalog-open-api-load-table-result
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: LoadTableResult
---
