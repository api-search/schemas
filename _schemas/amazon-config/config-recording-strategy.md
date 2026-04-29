---
description: Specifies the recording strategy of the configuration recorder.
layout: schema
name: RecordingStrategy
properties_list:
- description: ''
  name: useOnly
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-recording-strategy-schema.json
slug: config-recording-strategy
source_filename: config-recording-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-recording-strategy-schema.json\",\n  \"title\": \"RecordingStrategy\",\n  \"description\": \"Specifies the recording strategy of the configuration recorder.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"useOnly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingStrategyType\"\n        },\n        {\n          \"description\": \"<p>The recording strategy for the configuration recorder.</p> <ul> <li> <p>If you set this option to <code>ALL_SUPPORTED_RESOURCE_TYPES</code>, Config records configuration changes for all supported regional resource types. You also must set the <code>allSupported</code> field of <a href=\\\"https://docs.aws.amazon.com/config/latest/APIReference/API_RecordingGroup.html\\\">RecordingGroup</a> to <code>true</code>.</p> <p>When Config\
  \ adds support for a new type of regional resource, Config automatically starts recording resources of that type. For a list of supported resource types, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/resource-config-reference.html#supported-resources\\\">Supported Resource Types</a> in the <i>Config developer guide</i>.</p> </li> <li> <p>If you set this option to <code>INCLUSION_BY_RESOURCE_TYPES</code>, Config records configuration changes for only the resource types that you specify in the <code>resourceTypes</code> field of <a href=\\\"https://docs.aws.amazon.com/config/latest/APIReference/API_RecordingGroup.html\\\">RecordingGroup</a>.</p> </li> <li> <p>If you set this option to <code>EXCLUSION_BY_RESOURCE_TYPES</code>, Config records configuration changes for all supported resource types, except the resource types that you specify as exemptions to exclude from being recorded in the <code>resourceTypes</code> field of <a href=\\\"https://docs.aws.amazon.com/config/latest/APIReference/API_ExclusionByResourceTypes.html\\\
  \">ExclusionByResourceTypes</a>.</p> </li> </ul> <note> <p>The <code>recordingStrategy</code> field is optional when you set the <code>allSupported</code> field of <a href=\\\"https://docs.aws.amazon.com/config/latest/APIReference/API_RecordingGroup.html\\\">RecordingGroup</a> to <code>true</code>.</p> <p>The <code>recordingStrategy</code> field is optional when you list resource types in the <code>resourceTypes</code> field of <a href=\\\"https://docs.aws.amazon.com/config/latest/APIReference/API_RecordingGroup.html\\\">RecordingGroup</a>.</p> <p>The <code>recordingStrategy</code> field is required if you list resource types to exclude from recording in the <code>resourceTypes</code> field of <a href=\\\"https://docs.aws.amazon.com/config/latest/APIReference/API_ExclusionByResourceTypes.html\\\">ExclusionByResourceTypes</a>.</p> </note> <note> <p>If you choose <code>EXCLUSION_BY_RESOURCE_TYPES</code> for the recording strategy, the <code>exclusionByResourceTypes</code> field will override\
  \ other properties in the request.</p> <p>For example, even if you set <code>includeGlobalResourceTypes</code> to false, global resource types will still be automatically recorded in this option unless those resource types are specifically listed as exemptions in the <code>resourceTypes</code> field of <code>exclusionByResourceTypes</code>.</p> <p>By default, if you choose the <code>EXCLUSION_BY_RESOURCE_TYPES</code> recording strategy, when Config adds support for a new resource type in the Region where you set up the configuration recorder, including global resource types, Config starts recording resources of that type automatically.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-recording-strategy-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: RecordingStrategy
---
