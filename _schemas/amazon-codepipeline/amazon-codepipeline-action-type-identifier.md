---
description: Specifies the category, owner, provider, and version of the action type.
layout: schema
name: ActionTypeIdentifier
properties_list:
- description: ''
  name: category
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: provider
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-type-identifier-schema.json
slug: amazon-codepipeline-action-type-identifier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-identifier-schema.json\",\n  \"title\": \"ActionTypeIdentifier\",\n  \"description\": \"Specifies the category, owner, provider, and version of the action type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionCategory\"\n        },\n        {\n          \"description\": \"<p>Defines what kind of action can be taken in the stage, one of the following:</p> <ul> <li> <p> <code>Source</code> </p> </li> <li> <p> <code>Build</code> </p> </li> <li> <p> <code>Test</code> </p> </li> <li> <p> <code>Deploy</code> </p> </li> <li> <p> <code>Approval</code> </p> </li> <li> <p> <code>Invoke</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/ActionTypeOwner\"\n        },\n        {\n          \"description\": \"The creator of the action type being called: <code>AWS</code> or <code>ThirdParty</code>.\"\n        }\n      ]\n    },\n    \"provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionProvider\"\n        },\n        {\n          \"description\": \"The provider of the action type being called. The provider name is supplied when the action type is created.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"A string that describes the action type version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"owner\",\n    \"provider\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-identifier-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionTypeIdentifier
---
