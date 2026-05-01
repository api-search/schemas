---
description: DescribeConfigurationRevisionResponse schema from Amazon MSK API
layout: schema
name: DescribeConfigurationRevisionResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Revision
  type: object
- description: ''
  name: ServerProperties
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-describe-configuration-revision-response-schema.json
slug: msk-api-describe-configuration-revision-response
source_filename: msk-api-describe-configuration-revision-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-describe-configuration-revision-response-schema.json\",\n  \"title\": \"DescribeConfigurationRevisionResponse\",\n  \"description\": \"DescribeConfigurationRevisionResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) of the configuration.</p>\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"creationTime\"\n          },\n          \"\
  description\": \"\\n            <p>The time when the configuration was created.</p>\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"\\n            <p>The description of the configuration.</p>\"\n        }\n      ]\n    },\n    \"Revision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"revision\"\n          },\n          \"description\": \"\\n            <p>The revision number.</p>\"\n        }\n      ]\n    },\n    \"ServerProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__blob\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serverProperties\"\n          },\n          \"description\": \"\\n     \
  \       <p>Contents of the <filename>server.properties</filename> file. When using the API, you must ensure that the contents of the file are base64 encoded. \\n               When using the AWS Management Console, the SDK, or the AWS CLI, the contents of <filename>server.properties</filename> can be in plaintext.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-describe-configuration-revision-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DescribeConfigurationRevisionResponse
---
