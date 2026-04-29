---
description: DescribeSecurityProfileResponse schema
layout: schema
name: DescribeSecurityProfileResponse
properties_list:
- description: ''
  name: securityProfileName
  type: object
- description: ''
  name: securityProfileArn
  type: object
- description: ''
  name: securityProfileDescription
  type: object
- description: ''
  name: behaviors
  type: object
- description: ''
  name: alertTargets
  type: object
- description: ''
  name: additionalMetricsToRetain
  type: object
- description: ''
  name: additionalMetricsToRetainV2
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-security-profile-response-schema.json
slug: iot-core-describe-security-profile-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-security-profile-response-schema.json\",\n  \"title\": \"DescribeSecurityProfileResponse\",\n  \"description\": \"DescribeSecurityProfileResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"securityProfileName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityProfileName\"\n        },\n        {\n          \"description\": \"The name of the security profile.\"\n        }\n      ]\n    },\n    \"securityProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityProfileArn\"\n        },\n        {\n          \"description\": \"The ARN of the security profile.\"\n        }\n      ]\n    },\n    \"securityProfileDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityProfileDescription\"\
  \n        },\n        {\n          \"description\": \"A description of the security profile (associated with the security profile when it was created or updated).\"\n        }\n      ]\n    },\n    \"behaviors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Behaviors\"\n        },\n        {\n          \"description\": \"Specifies the behaviors that, when violated by a device (thing), cause an alert.\"\n        }\n      ]\n    },\n    \"alertTargets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertTargets\"\n        },\n        {\n          \"description\": \"Where the alerts are sent. (Alerts are always sent to the console.)\"\n        }\n      ]\n    },\n    \"additionalMetricsToRetain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalMetricsToRetainList\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"<p> <i>Please use <a>DescribeSecurityProfileResponse$additionalMetricsToRetainV2</a>\
  \ instead.</i> </p> <p>A list of metrics whose data is retained (stored). By default, data is retained for any metric used in the profile's <code>behaviors</code>, but it is also retained for any metric specified here.</p>Use additionalMetricsToRetainV2.\"\n        }\n      ]\n    },\n    \"additionalMetricsToRetainV2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdditionalMetricsToRetainV2List\"\n        },\n        {\n          \"description\": \"A list of metrics whose data is retained (stored). By default, data is retained for any metric used in the profile's behaviors, but it is also retained for any metric specified here.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the security profile. A new version is generated whenever the security profile is updated.\"\n        }\n      ]\n    },\n    \"\
  creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the security profile was created.\"\n        }\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time the security profile was last modified.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-security-profile-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeSecurityProfileResponse
---
