---
description: UpdateEnvironmentRequest schema from AWS Mainframe Modernization API
layout: schema
name: UpdateEnvironmentRequest
properties_list:
- description: ''
  name: applyDuringMaintenanceWindow
  type: object
- description: ''
  name: desiredCapacity
  type: object
- description: ''
  name: engineVersion
  type: object
- description: ''
  name: instanceType
  type: object
- description: ''
  name: preferredMaintenanceWindow
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-update-environment-request-schema.json
slug: amazon-mainframe-modernization-update-environment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-update-environment-request-schema.json\",\n  \"title\": \"UpdateEnvironmentRequest\",\n  \"description\": \"UpdateEnvironmentRequest schema from AWS Mainframe Modernization API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applyDuringMaintenanceWindow\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether to update the runtime environment during the maintenance window. The default is false. Currently, Amazon Web Services Mainframe Modernization accepts the <code>engineVersion</code> parameter only if <code>applyDuringMaintenanceWindow</code> is true. If any parameter other than <code>engineVersion</code> is provided in <code>UpdateEnvironmentRequest</code>,\
  \ it will fail if <code>applyDuringMaintenanceWindow</code> is set to true.\"\n        }\n      ]\n    },\n    \"desiredCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CapacityValue\"\n        },\n        {\n          \"description\": \"The desired capacity for the runtime environment to update. The minimum possible value is 0 and the maximum is 100.\"\n        }\n      ]\n    },\n    \"engineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineVersion\"\n        },\n        {\n          \"description\": \"The version of the runtime engine for the runtime environment.\"\n        }\n      ]\n    },\n    \"instanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String20\"\n        },\n        {\n          \"description\": \"The instance type for the runtime environment to update.\"\n        }\n      ]\n    },\n    \"preferredMaintenanceWindow\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Configures the maintenance window you want for the runtime environment. If you do not provide a value, a random system-generated value will be assigned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-update-environment-request-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: UpdateEnvironmentRequest
---
