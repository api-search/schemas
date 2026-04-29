---
description: Contains the status of a component version in the IoT Greengrass service.
layout: schema
name: CloudComponentStatus
properties_list:
- description: ''
  name: componentState
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: errors
  type: object
- description: ''
  name: vendorGuidance
  type: object
- description: ''
  name: vendorGuidanceMessage
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-cloud-component-status-schema.json
slug: iot-greengrass-cloud-component-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-cloud-component-status-schema.json\",\n  \"title\": \"CloudComponentStatus\",\n  \"description\": \"Contains the status of a component version in the IoT Greengrass service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"componentState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudComponentState\"\n        },\n        {\n          \"description\": \"The state of the component version.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A message that communicates details, such as errors, about the status of the component version.\"\n        }\n      ]\n    },\n    \"errors\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/StringMap\"\n        },\n        {\n          \"description\": \"A dictionary of errors that communicate why the component version is in an error state. For example, if IoT Greengrass can't access an artifact for the component version, then <code>errors</code> contains the artifact's URI as a key, and the error message as the value for that key.\"\n        }\n      ]\n    },\n    \"vendorGuidance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VendorGuidance\"\n        },\n        {\n          \"description\": \"<p>The vendor guidance state for the component version. This state indicates whether the component version has any issues that you should consider before you deploy it. The vendor guidance state can be:</p> <ul> <li> <p> <code>ACTIVE</code> \\u2013 This component version is available and recommended for use.</p> </li> <li> <p> <code>DISCONTINUED</code> \\u2013 This component version has been\
  \ discontinued by its publisher. You can deploy this component version, but we recommend that you use a different version of this component.</p> </li> <li> <p> <code>DELETED</code> \\u2013 This component version has been deleted by its publisher, so you can't deploy it. If you have any existing deployments that specify this component version, those deployments will fail.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"vendorGuidanceMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A message that communicates details about the vendor guidance state of the component version. This message communicates why a component version is discontinued or deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-cloud-component-status-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: CloudComponentStatus
---
