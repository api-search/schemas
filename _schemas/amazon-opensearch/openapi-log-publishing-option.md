---
description: 'Log Publishing option that is set for given domain. <br/>Attributes and their details: <ul> <li>CloudWatchLogsLogGroupArn: ARN of the Cloudwatch log group to which log needs to be published.</li> <li>Enabled: Whether the log publishing for given log type is enabled or not</li> </ul>'
layout: schema
name: LogPublishingOption
properties_list:
- description: ''
  name: CloudWatchLogsLogGroupArn
  type: object
- description: ''
  name: Enabled
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-log-publishing-option-schema.json
slug: openapi-log-publishing-option
source_filename: openapi-log-publishing-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-log-publishing-option-schema.json\",\n  \"title\": \"LogPublishingOption\",\n  \"description\": \"Log Publishing option that is set for given domain. <br/>Attributes and their details: <ul> <li>CloudWatchLogsLogGroupArn: ARN of the Cloudwatch log group to which log needs to be published.</li> <li>Enabled: Whether the log publishing for given log type is enabled or not</li> </ul> \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudWatchLogsLogGroupArn\": {\n      \"$ref\": \"#/components/schemas/CloudWatchLogsLogGroupArn\"\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" Specifies whether given log publishing option is enabled or not.\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-log-publishing-option-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: LogPublishingOption
---
