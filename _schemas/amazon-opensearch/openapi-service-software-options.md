---
description: The current options of an Elasticsearch domain service software options.
layout: schema
name: ServiceSoftwareOptions
properties_list:
- description: ''
  name: CurrentVersion
  type: object
- description: ''
  name: NewVersion
  type: object
- description: ''
  name: UpdateAvailable
  type: object
- description: ''
  name: Cancellable
  type: object
- description: ''
  name: UpdateStatus
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: AutomatedUpdateDate
  type: object
- description: ''
  name: OptionalDeployment
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-service-software-options-schema.json
slug: openapi-service-software-options
source_filename: openapi-service-software-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-service-software-options-schema.json\",\n  \"title\": \"ServiceSoftwareOptions\",\n  \"description\": \"The current options of an Elasticsearch domain service software options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CurrentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The current service software version that is present on the domain.\"\n        }\n      ]\n    },\n    \"NewVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The new service software version if one is available.\"\n        }\n      ]\n    },\n    \"UpdateAvailable\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<code>True</code> if you are able to update you service software version. <code>False</code> if you are not able to update your service software version. \"\n        }\n      ]\n    },\n    \"Cancellable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<code>True</code> if you are able to cancel your service software version update. <code>False</code> if you are not able to cancel your service software version. \"\n        }\n      ]\n    },\n    \"UpdateStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentStatus\"\n        },\n        {\n          \"description\": \"The status of your service software update. This field can take the following values: <code>ELIGIBLE</code>, <code>PENDING_UPDATE</code>, <code>IN_PROGRESS</code>, <code>COMPLETED</code>, and <code>NOT_ELIGIBLE</code>.\"\
  \n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The description of the <code>UpdateStatus</code>.\"\n        }\n      ]\n    },\n    \"AutomatedUpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentCloseDateTimeStamp\"\n        },\n        {\n          \"description\": \"Timestamp, in Epoch time, until which you can manually request a service software update. After this date, we automatically update your service software.\"\n        }\n      ]\n    },\n    \"OptionalDeployment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<code>True</code> if a service software is never automatically updated. <code>False</code> if a service software is automatically updated after <code>AutomatedUpdateDate</code>. \"\n   \
  \     }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-service-software-options-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ServiceSoftwareOptions
---
