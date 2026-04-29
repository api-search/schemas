---
description: Summary counts of each Proton resource type.
layout: schema
name: CountsSummary
properties_list:
- description: ''
  name: components
  type: object
- description: ''
  name: environmentTemplates
  type: object
- description: ''
  name: environments
  type: object
- description: ''
  name: pipelines
  type: object
- description: ''
  name: serviceInstances
  type: object
- description: ''
  name: serviceTemplates
  type: object
- description: ''
  name: services
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-counts-summary-schema.json
slug: amazon-proton-counts-summary
source_filename: amazon-proton-counts-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-counts-summary-schema.json\",\n  \"title\": \"CountsSummary\",\n  \"description\": \"Summary counts of each Proton resource type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"components\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCountsSummary\"\n        },\n        {\n          \"description\": \"<p>The total number of components in the Amazon Web Services account.</p> <p>The semantics of the <code>components</code> field are different from the semantics of results for other infrastructure-provisioning resources. That's because at this time components don't have associated templates, therefore they don't have the concept of staleness. The <code>components</code> object will only contain <code>total</code> and <code>failed</code> members.</p>\"\
  \n        }\n      ]\n    },\n    \"environmentTemplates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCountsSummary\"\n        },\n        {\n          \"description\": \"The total number of environment templates in the Amazon Web Services account. The <code>environmentTemplates</code> object will only contain <code>total</code> members.\"\n        }\n      ]\n    },\n    \"environments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCountsSummary\"\n        },\n        {\n          \"description\": \"The staleness counts for Proton environments in the Amazon Web Services account. The <code>environments</code> object will only contain <code>total</code> members.\"\n        }\n      ]\n    },\n    \"pipelines\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCountsSummary\"\n        },\n        {\n          \"description\": \"The staleness counts for Proton pipelines\
  \ in the Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"serviceInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCountsSummary\"\n        },\n        {\n          \"description\": \"The staleness counts for Proton service instances in the Amazon Web Services account.\"\n        }\n      ]\n    },\n    \"serviceTemplates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCountsSummary\"\n        },\n        {\n          \"description\": \"The total number of service templates in the Amazon Web Services account. The <code>serviceTemplates</code> object will only contain <code>total</code> members.\"\n        }\n      ]\n    },\n    \"services\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCountsSummary\"\n        },\n        {\n          \"description\": \"The staleness counts for Proton services in the Amazon Web Services account.\"\n        }\n\
  \      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-counts-summary-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: CountsSummary
---
