---
description: SetCurrentViewVersionUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: SetCurrentViewVersionUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: The view version id to set as current, or -1 to set last added view version id
  name: view-version-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-set-current-view-version-update-schema.json
slug: rest-catalog-open-api-set-current-view-version-update
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SetCurrentViewVersionUpdate
---
