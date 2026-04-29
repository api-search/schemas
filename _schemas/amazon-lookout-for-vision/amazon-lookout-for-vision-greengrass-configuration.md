---
description: <p>Configuration information for the AWS IoT Greengrass component created in a model packaging job. For more information, see <a>StartModelPackagingJob</a>. </p> <note> <p>You can't specify a component with the same <code>ComponentName</code> and <code>Componentversion</code> as an existing component with the same component name and component version.</p> </note>
layout: schema
name: GreengrassConfiguration
properties_list:
- description: ''
  name: CompilerOptions
  type: object
- description: ''
  name: TargetDevice
  type: object
- description: ''
  name: TargetPlatform
  type: object
- description: ''
  name: S3OutputLocation
  type: object
- description: ''
  name: ComponentName
  type: object
- description: ''
  name: ComponentVersion
  type: object
- description: ''
  name: ComponentDescription
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-greengrass-configuration-schema.json
slug: amazon-lookout-for-vision-greengrass-configuration
source_filename: amazon-lookout-for-vision-greengrass-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-greengrass-configuration-schema.json\",\n  \"title\": \"GreengrassConfiguration\",\n  \"description\": \"<p>Configuration information for the AWS IoT Greengrass component created in a model packaging job. For more information, see <a>StartModelPackagingJob</a>. </p> <note> <p>You can't specify a component with the same <code>ComponentName</code> and <code>Componentversion</code> as an existing component with the same component name and component version.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CompilerOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompilerOptions\"\n        },\n        {\n          \"description\": \"<p>Additional compiler options for the Greengrass component. Currently, only NVIDIA\
  \ Graphics Processing Units (GPU) and CPU accelerators are supported. If you specify <code>TargetDevice</code>, don't specify <code>CompilerOptions</code>.</p> <p>For more information, see <i>Compiler options</i> in the Amazon Lookout for Vision Developer Guide. </p>\"\n        }\n      ]\n    },\n    \"TargetDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetDevice\"\n        },\n        {\n          \"description\": \"The target device for the model. Currently the only supported value is <code>jetson_xavier</code>. If you specify <code>TargetDevice</code>, you can't specify <code>TargetPlatform</code>. \"\n        }\n      ]\n    },\n    \"TargetPlatform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetPlatform\"\n        },\n        {\n          \"description\": \"The target platform for the model. If you specify <code>TargetPlatform</code>, you can't specify <code>TargetDevice</code>. \"\n        }\n   \
  \   ]\n    },\n    \"S3OutputLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \" An S3 location in which Lookout for Vision stores the component artifacts. \"\n        }\n      ]\n    },\n    \"ComponentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentName\"\n        },\n        {\n          \"description\": \" A name for the AWS IoT Greengrass component. \"\n        }\n      ]\n    },\n    \"ComponentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersion\"\n        },\n        {\n          \"description\": \"A Version for the AWS IoT Greengrass component. If you don't provide a value, a default value of <code> <i>Model Version</i>.0.0</code> is used. \"\n        }\n      ]\n    },\n    \"ComponentDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentDescription\"\
  \n        },\n        {\n          \"description\": \" A description for the AWS IoT Greengrass component. \"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \" A set of tags (key-value pairs) that you want to attach to the AWS IoT Greengrass component. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3OutputLocation\",\n    \"ComponentName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-greengrass-configuration-schema.json
tags:
- AWS
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: GreengrassConfiguration
---
