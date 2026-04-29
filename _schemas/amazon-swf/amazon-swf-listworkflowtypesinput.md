---
description: ''
layout: schema
name: ListWorkflowTypesInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: registrationStatus
  type: object
- description: ''
  name: nextPageToken
  type: object
- description: ''
  name: maximumPageSize
  type: object
- description: ''
  name: reverseOrder
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-listworkflowtypesinput-schema.json
slug: amazon-swf-listworkflowtypesinput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"registrationStatus\"\n  ],\n  \"title\": \"ListWorkflowTypesInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain in which the workflow types have been registered.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"If specified, lists the workflow type with this name.\"\n        }\n      ]\n    },\n    \"registrationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegistrationStatus\"\n        },\n        {\n          \"description\": \"Specifies the registration status of the workflow types to list.\"\n        }\n      ]\n    },\n    \"nextPageToken\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"<p>If <code>NextPageToken</code> is returned there are more results available. The value of <code>NextPageToken</code> is a unique pagination token for each page. Make the call again using the returned token to retrieve the next page. Keep all other arguments unchanged. Each pagination token expires after 24 hours. Using an expired pagination token will return a <code>400</code> error: \\\"<code>Specified token has exceeded its maximum lifetime</code>\\\". </p> <p>The configured <code>maximumPageSize</code> determines how many results can be returned in a single call. </p>\"\n        }\n      ]\n    },\n    \"maximumPageSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of results that are returned per call. Use <code>nextPageToken</code> to obtain further pages\
  \ of results. \"\n        }\n      ]\n    },\n    \"reverseOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReverseOrder\"\n        },\n        {\n          \"description\": \"When set to <code>true</code>, returns the results in reverse order. By default the results are returned in ascending alphabetical order of the <code>name</code> of the workflow types.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-listworkflowtypesinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ListWorkflowTypesInput
---
