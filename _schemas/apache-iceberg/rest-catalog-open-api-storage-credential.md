---
description: StorageCredential schema from Apache Iceberg REST Catalog API
layout: schema
name: StorageCredential
properties_list:
- description: Indicates a storage location prefix where the credential is relevant. Clients should choose the most specific prefix (by selecting the longest prefix) if several credentials of the same type are avail
  name: prefix
  type: string
- description: ''
  name: config
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-storage-credential-schema.json
slug: rest-catalog-open-api-storage-credential
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: StorageCredential
---
