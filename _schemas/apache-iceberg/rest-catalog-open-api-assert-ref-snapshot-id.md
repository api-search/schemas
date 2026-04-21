---
description: The table branch or tag identified by the requirement's `ref` must reference the requirement's `snapshot-id`. The `snapshot-id` field is required in this object, but in the case of a `null` the ref must not already exist.
layout: schema
name: AssertRefSnapshotId
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: ref
  type: string
- description: ''
  name: snapshot-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assert-ref-snapshot-id-schema.json
slug: rest-catalog-open-api-assert-ref-snapshot-id
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssertRefSnapshotId
---
