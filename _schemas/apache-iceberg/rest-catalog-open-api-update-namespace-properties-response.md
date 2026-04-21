---
description: UpdateNamespacePropertiesResponse schema from Apache Iceberg REST Catalog API
layout: schema
name: UpdateNamespacePropertiesResponse
properties_list:
- description: List of property keys that were added or updated
  name: updated
  type: array
- description: List of properties that were removed
  name: removed
  type: array
- description: List of properties requested for removal that were not found in the namespace's properties. Represents a partial success response. Server's do not need to implement this.
  name: missing
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-update-namespace-properties-response-schema.json
slug: rest-catalog-open-api-update-namespace-properties-response
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: UpdateNamespacePropertiesResponse
---
