---
description: <p>Describes a configuration revision.</p>
layout: schema
name: ConfigurationRevision
properties_list:
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Revision
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-configuration-revision-schema.json
slug: msk-api-configuration-revision
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-configuration-revision-schema.json\",\n  \"title\": \"ConfigurationRevision\",\n  \"description\": \"\\n            <p>Describes a configuration revision.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"creationTime\"\n          },\n          \"description\": \"\\n            <p>The time when the configuration revision was created.</p>\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"\\n    \
  \        <p>The description of the configuration revision.</p>\"\n        }\n      ]\n    },\n    \"Revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"revision\"\n          },\n          \"description\": \"\\n            <p>The revision number.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Revision\",\n    \"CreationTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-configuration-revision-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ConfigurationRevision
---
