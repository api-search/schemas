---
description: TableUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: TableUpdate
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-table-update-schema.json
slug: rest-catalog-open-api-table-update
source_filename: rest-catalog-open-api-table-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-table-update-schema.json\",\n  \"title\": \"TableUpdate\",\n  \"description\": \"TableUpdate schema from Apache Iceberg REST Catalog API\",\n  \"anyOf\": [\n    {\n      \"$ref\": \"#/components/schemas/AssignUUIDUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/UpgradeFormatVersionUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/AddSchemaUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetCurrentSchemaUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/AddPartitionSpecUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetDefaultSpecUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/AddSortOrderUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetDefaultSortOrderUpdate\"\n    },\n    {\n\
  \      \"$ref\": \"#/components/schemas/AddSnapshotUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetSnapshotRefUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RemoveSnapshotsUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RemoveSnapshotRefUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetLocationUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetPropertiesUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RemovePropertiesUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetStatisticsUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RemoveStatisticsUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetPartitionStatisticsUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RemovePartitionStatisticsUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RemovePartitionSpecsUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RemoveSchemasUpdate\"\
  \n    },\n    {\n      \"$ref\": \"#/components/schemas/AddEncryptionKeyUpdate\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RemoveEncryptionKeyUpdate\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-table-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: TableUpdate
---
