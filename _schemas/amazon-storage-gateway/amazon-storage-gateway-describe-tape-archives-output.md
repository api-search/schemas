---
description: DescribeTapeArchivesOutput
layout: schema
name: DescribeTapeArchivesOutput
properties_list:
- description: ''
  name: TapeArchives
  type: object
- description: ''
  name: Marker
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-tape-archives-output-schema.json
slug: amazon-storage-gateway-describe-tape-archives-output
source_filename: amazon-storage-gateway-describe-tape-archives-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tape-archives-output-schema.json\",\n  \"title\": \"DescribeTapeArchivesOutput\",\n  \"description\": \"DescribeTapeArchivesOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeArchives\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeArchives\"\n        },\n        {\n          \"description\": \"An array of virtual tape objects in the virtual tape shelf (VTS). The description includes of the Amazon Resource Name (ARN) of the virtual tapes. The information returned includes the Amazon Resource Names (ARNs) of the tapes, size of the tapes, status of the tapes, progress of the description, and tape barcode.\"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\
  \n        },\n        {\n          \"description\": \"An opaque string that indicates the position at which the virtual tapes that were fetched for description ended. Use this marker in your next request to fetch the next set of virtual tapes in the virtual tape shelf (VTS). If there are no more virtual tapes to describe, this field does not appear in the response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tape-archives-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeTapeArchivesOutput
---
