---
description: Describes a quota for an Amazon Web Services account, for example the number of replication instances allowed.
layout: schema
name: AccountQuota
properties_list:
- description: ''
  name: AccountQuotaName
  type: object
- description: ''
  name: Used
  type: object
- description: ''
  name: Max
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-account-quota-schema.json
slug: amazon-dms-account-quota
source_filename: amazon-dms-account-quota-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-account-quota-schema.json\",\n  \"title\": \"AccountQuota\",\n  \"description\": \"Describes a quota for an Amazon Web Services account, for example the number of replication instances allowed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountQuotaName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the DMS quota for this Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"Used\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The amount currently used toward the quota maximum.\"\n        }\n      ]\n    },\n    \"Max\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The maximum allowed value for the quota.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-account-quota-schema.json
tags:
- Data Replication
- Database
- Database Migration
- Migration
title: AccountQuota
---
