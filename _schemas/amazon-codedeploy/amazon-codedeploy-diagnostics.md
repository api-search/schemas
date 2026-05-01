---
description: Diagnostic information about executable scripts that are part of a deployment.
layout: schema
name: Diagnostics
properties_list:
- description: ''
  name: errorCode
  type: object
- description: ''
  name: scriptName
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: logTail
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-diagnostics-schema.json
slug: amazon-codedeploy-diagnostics
source_filename: amazon-codedeploy-diagnostics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-diagnostics-schema.json\",\n  \"title\": \"Diagnostics\",\n  \"description\": \"Diagnostic information about executable scripts that are part of a deployment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleErrorCode\"\n        },\n        {\n          \"description\": \"<p>The associated error code:</p> <ul> <li> <p>Success: The specified script ran.</p> </li> <li> <p>ScriptMissing: The specified script was not found in the specified location.</p> </li> <li> <p>ScriptNotExecutable: The specified script is not a recognized executable file type.</p> </li> <li> <p>ScriptTimedOut: The specified script did not finish running in the specified time period.</p> </li> <li> <p>ScriptFailed:\
  \ The specified script failed to run as expected.</p> </li> <li> <p>UnknownError: The specified script did not run for an unknown reason.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"scriptName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScriptName\"\n        },\n        {\n          \"description\": \"The name of the script.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleMessage\"\n        },\n        {\n          \"description\": \"The message associated with the error.\"\n        }\n      ]\n    },\n    \"logTail\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogTail\"\n        },\n        {\n          \"description\": \"<p>The last portion of the diagnostic log.</p> <p>If available, CodeDeploy returns up to the last 4 KB of the diagnostic log.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-diagnostics-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: Diagnostics
---
