---
description: Contains information about a component version that is compatible to run on a Greengrass core device.
layout: schema
name: ResolvedComponentVersion
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: componentName
  type: object
- description: ''
  name: componentVersion
  type: object
- description: ''
  name: recipe
  type: object
- description: ''
  name: vendorGuidance
  type: object
- description: ''
  name: message
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-resolved-component-version-schema.json
slug: iot-greengrass-resolved-component-version
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-resolved-component-version-schema.json\",\n  \"title\": \"ResolvedComponentVersion\",\n  \"description\": \"Contains information about a component version that is compatible to run on a Greengrass core device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the component version.\"\n        }\n      ]\n    },\n    \"componentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentNameString\"\n        },\n        {\n          \"description\": \"The name of the component.\"\n \
  \       }\n      ]\n    },\n    \"componentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionString\"\n        },\n        {\n          \"description\": \"The version of the component.\"\n        }\n      ]\n    },\n    \"recipe\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeBlob\"\n        },\n        {\n          \"description\": \"The recipe of the component version.\"\n        }\n      ]\n    },\n    \"vendorGuidance\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VendorGuidance\"\n        },\n        {\n          \"description\": \"<p>The vendor guidance state for the component version. This state indicates whether the component version has any issues that you should consider before you deploy it. The vendor guidance state can be:</p> <ul> <li> <p> <code>ACTIVE</code> \\u2013 This component version is available and recommended for use.</p> </li> <li> <p> <code>DISCONTINUED</code>\
  \ \\u2013 This component version has been discontinued by its publisher. You can deploy this component version, but we recommend that you use a different version of this component.</p> </li> <li> <p> <code>DELETED</code> \\u2013 This component version has been deleted by its publisher, so you can't deploy it. If you have any existing deployments that specify this component version, those deployments will fail.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"A message that communicates details about the vendor guidance state of the component version. This message communicates why a component version is discontinued or deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-resolved-component-version-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ResolvedComponentVersion
---
