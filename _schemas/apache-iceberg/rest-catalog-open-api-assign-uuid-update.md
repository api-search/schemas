---
description: Assigning a UUID to a table/view should only be done when creating the table/view. It is not safe to re-assign the UUID if a table/view already has a UUID assigned
layout: schema
name: AssignUUIDUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: uuid
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-assign-uuid-update-schema.json
slug: rest-catalog-open-api-assign-uuid-update
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AssignUUIDUpdate
---
