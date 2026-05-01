---
description: <p> Status of the advanced options for the specified Elasticsearch domain. Currently, the following advanced options are available:</p> <ul> <li>Option to allow references to indices in an HTTP request body. Must be <code>false</code> when configuring access to individual sub-resources. By default, the value is <code>true</code>. See <a href="http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-advanced-options" target="_blank">Configuration Advanced Options</a> for more information.</li> <li>Option to specify the percentage of heap space that is allocated to field data. By default, this setting is unbounded.</li> </ul> <p>For more information, see <a href="http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-advanced-options">Configuring Advanced Options</a>.</p>
layout: schema
name: AdvancedOptionsStatus
properties_list:
- description: ''
  name: Options
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-advanced-options-status-schema.json
slug: openapi-advanced-options-status
source_filename: openapi-advanced-options-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-advanced-options-status-schema.json\",\n  \"title\": \"AdvancedOptionsStatus\",\n  \"description\": \"<p> Status of the advanced options for the specified Elasticsearch domain. Currently, the following advanced options are available:</p> <ul> <li>Option to allow references to indices in an HTTP request body. Must be <code>false</code> when configuring access to individual sub-resources. By default, the value is <code>true</code>. See <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-advanced-options\\\" target=\\\"_blank\\\">Configuration Advanced Options</a> for more information.</li> <li>Option to specify the percentage of heap space that is allocated to field data. By default, this setting is unbounded.</li>\
  \ </ul> <p>For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-advanced-options\\\">Configuring Advanced Options</a>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Options\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedOptions\"\n        },\n        {\n          \"description\": \" Specifies the status of advanced options for the specified Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionStatus\"\n        },\n        {\n          \"description\": \" Specifies the status of <code>OptionStatus</code> for advanced options for the specified Elasticsearch domain.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Options\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-advanced-options-status-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: AdvancedOptionsStatus
---
