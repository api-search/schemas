---
description: SetDefaultSpecUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: SetDefaultSpecUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: Partition spec ID to set as the default, or -1 to set last added spec
  name: spec-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-set-default-spec-update-schema.json
slug: rest-catalog-open-api-set-default-spec-update
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SetDefaultSpecUpdate
---
