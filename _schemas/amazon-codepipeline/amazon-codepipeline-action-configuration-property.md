---
description: Represents information about an action configuration property.
layout: schema
name: ActionConfigurationProperty
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: required
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: secret
  type: object
- description: ''
  name: queryable
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-configuration-property-schema.json
slug: amazon-codepipeline-action-configuration-property
source_filename: amazon-codepipeline-action-configuration-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-configuration-property-schema.json\",\n  \"title\": \"ActionConfigurationProperty\",\n  \"description\": \"Represents information about an action configuration property.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionConfigurationKey\"\n        },\n        {\n          \"description\": \"The name of the action configuration property.\"\n        }\n      ]\n    },\n    \"required\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the configuration property is a required value.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the configuration property is a key.\"\n        }\n      ]\n    },\n    \"secret\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Whether the configuration property is secret. Secrets are hidden from all calls except for <code>GetJobDetails</code>, <code>GetThirdPartyJobDetails</code>, <code>PollForJobs</code>, and <code>PollForThirdPartyJobs</code>.</p> <p>When updating a pipeline, passing * * * * * without changing any other values of the action preserves the previous value of the secret.</p>\"\n        }\n      ]\n    },\n    \"queryable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Indicates that the property is used with <code>PollForJobs</code>. When creating a custom action, an action can have up\
  \ to one queryable property. If it has one, that property must be both required and not secret.</p> <p>If you create a pipeline with a custom action type, and that custom action contains a queryable property, the value for that configuration property is subject to other restrictions. The value must be less than or equal to twenty (20) characters. The value can contain only alphanumeric characters, underscores, and hyphens.</p>\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the action configuration property that is displayed to users.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionConfigurationPropertyType\"\n        },\n        {\n          \"description\": \"The type of the configuration property.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"name\",\n    \"required\",\n    \"key\",\n    \"secret\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-configuration-property-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionConfigurationProperty
---
