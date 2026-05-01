---
description: DescribeConfigurationRevisionResponse schema from Amazon MQ API
layout: schema
name: DescribeConfigurationRevisionResponse
properties_list:
- description: ''
  name: ConfigurationId
  type: object
- description: ''
  name: Created
  type: object
- description: ''
  name: Data
  type: object
- description: ''
  name: Description
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-describe-configuration-revision-response-schema.json
slug: mq-api-describe-configuration-revision-response
source_filename: mq-api-describe-configuration-revision-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-describe-configuration-revision-response-schema.json\",\n  \"title\": \"DescribeConfigurationRevisionResponse\",\n  \"description\": \"DescribeConfigurationRevisionResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"configurationId\"\n          },\n          \"description\": \"Required. The unique ID that Amazon MQ generates for the configuration.\"\n        }\n      ]\n    },\n    \"Created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"created\"\n          },\n    \
  \      \"description\": \"Required. The date and time of the configuration.\"\n        }\n      ]\n    },\n    \"Data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"data\"\n          },\n          \"description\": \"Required. The base64-encoded XML configuration.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"The description of the configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-describe-configuration-revision-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DescribeConfigurationRevisionResponse
---
