---
description: Details about the ingest state of a datasource package
layout: schema
name: DatasourcePackageIngestDetail
properties_list:
- description: Details on which data source packages are ingested for a member account.
  name: DatasourcePackageIngestState
  type: string
- description: The date a data source package type was last updated for a member account.
  name: LastIngestStateChange
  type: object
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-datasource-package-ingest-detail-schema.json
slug: amazon-detective-datasource-package-ingest-detail
source_filename: amazon-detective-datasource-package-ingest-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-datasource-package-ingest-detail-schema.json\",\n  \"title\": \"DatasourcePackageIngestDetail\",\n  \"description\": \"Details about the ingest state of a datasource package\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatasourcePackageIngestState\": {\n      \"type\": \"string\",\n      \"description\": \"Details on which data source packages are ingested for a member account.\",\n      \"enum\": [\n        \"STARTED\",\n        \"STOPPED\",\n        \"DISABLED\"\n      ]\n    },\n    \"LastIngestStateChange\": {\n      \"type\": \"object\",\n      \"description\": \"The date a data source package type was last updated for a member account.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/TimestampForCollection\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-datasource-package-ingest-detail-schema.json
tags:
- Forensics
- Investigation
- Security
title: DatasourcePackageIngestDetail
---
