---
description: The platform on which a model runs on an AWS IoT Greengrass core device.
layout: schema
name: TargetPlatform
properties_list:
- description: ''
  name: Os
  type: object
- description: ''
  name: Arch
  type: object
- description: ''
  name: Accelerator
  type: object
provider_name: Amazon Lookout for Vision
provider_slug: amazon-lookout-for-vision
schema_file: json-schema/amazon-lookout-for-vision-target-platform-schema.json
slug: amazon-lookout-for-vision-target-platform
source_filename: amazon-lookout-for-vision-target-platform-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-target-platform-schema.json\",\n  \"title\": \"TargetPlatform\",\n  \"description\": \"The platform on which a model runs on an AWS IoT Greengrass core device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Os\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetPlatformOs\"\n        },\n        {\n          \"description\": \"The target operating system for the model. Linux is the only operating system that is currently supported. \"\n        }\n      ]\n    },\n    \"Arch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetPlatformArch\"\n        },\n        {\n          \"description\": \"The target architecture for the model. The currently supported architectures are X86_64 (64-bit version\
  \ of the x86 instruction set) and ARM_64 (ARMv8 64-bit CPU). \"\n        }\n      ]\n    },\n    \"Accelerator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetPlatformAccelerator\"\n        },\n        {\n          \"description\": \"<p>The target accelerator for the model. Currently, Amazon Lookout for Vision only supports NVIDIA (Nvidia graphics processing unit) and CPU accelerators. If you specify NVIDIA as an accelerator, you must also specify the <code>gpu-code</code>, <code>trt-ver</code>, and <code>cuda-ver</code> compiler options. If you don't specify an accelerator, Lookout for Vision uses the CPU for compilation and we highly recommend that you use the <a>GreengrassConfiguration$CompilerOptions</a> field. For example, you can use the following compiler options for CPU: </p> <ul> <li> <p> <code>mcpu</code>: CPU micro-architecture. For example, <code>{'mcpu': 'skylake-avx512'}</code> </p> </li> <li> <p> <code>mattr</code>: CPU flags. For example,\
  \ <code>{'mattr': ['+neon', '+vfpv4']}</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Os\",\n    \"Arch\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-vision/refs/heads/main/json-schema/amazon-lookout-for-vision-target-platform-schema.json
tags:
- Computer Vision
- Machine Learning
- Manufacturing
- Quality Inspection
- Anomaly Detection
title: TargetPlatform
---
