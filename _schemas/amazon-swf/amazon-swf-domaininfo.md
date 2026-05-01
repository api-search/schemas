---
description: Contains general information about a domain.
layout: schema
name: DomainInfo
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: arn
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-domaininfo-schema.json
slug: amazon-swf-domaininfo
source_filename: amazon-swf-domaininfo-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain. This name is unique within the account.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the domain:</p> <ul> <li> <p> <code>REGISTERED</code> \\u2013 The domain is properly registered and available. You can use this domain for registering types and creating new workflow executions. </p> </li> <li> <p> <code>DEPRECATED</code> \\u2013 The domain was deprecated using <a>DeprecateDomain</a>, but is still in use. You should not create new workflow executions in this domain. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"description\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the domain provided through <a>RegisterDomain</a>.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the domain.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains general information about a domain.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DomainInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-domaininfo-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: DomainInfo
---
