---
description: ValueMap schema from Apache Iceberg REST Catalog API
layout: schema
name: ValueMap
properties_list:
- description: List of integer column ids for each corresponding value
  name: keys
  type: array
- description: List of primitive type values, matched to 'keys' by index
  name: values
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-value-map-schema.json
slug: rest-catalog-open-api-value-map
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ValueMap
---
