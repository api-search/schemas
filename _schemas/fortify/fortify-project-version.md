---
description: Represents a project version (application version) in Fortify Software Security Center. Project versions are the primary unit of work in SSC, containing scan artifacts, issue data, and audit information for a specific version of an application.
layout: schema
name: Fortify Project Version
properties_list:
- description: Unique identifier of the project version
  name: id
  type: integer
- description: Version name
  name: name
  type: string
- description: Version description
  name: description
  type: string
- description: Whether the version is active
  name: active
  type: boolean
- description: Whether the version has been committed (activated for use)
  name: committed
  type: boolean
- description: Parent project reference
  name: project
  type: object
- description: Username of the creator
  name: createdBy
  type: string
- description: Date when the version was created
  name: creationDate
  type: string
- description: Issue template identifier for this version
  name: issueTemplateId
  type: string
- description: Current processing state of the version
  name: currentState
  type: object
- description: Attribute values assigned to this version
  name: attributes
  type: array
provider_name: Fortify
provider_slug: fortify
schema_file: json-schema/fortify-project-version-schema.json
slug: fortify-project-version
source_filename: fortify-project-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/fortify/json-schema/fortify-project-version-schema.json\",\n  \"title\": \"Fortify Project Version\",\n  \"description\": \"Represents a project version (application version) in Fortify Software Security Center. Project versions are the primary unit of work in SSC, containing scan artifacts, issue data, and audit information for a specific version of an application.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unique identifier of the project version\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Version name\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Version description\"\n    },\n    \"active\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the version is active\",\n      \"default\": true\n    },\n    \"committed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the version has been committed (activated for use)\",\n      \"default\": false\n    },\n    \"project\": {\n      \"type\": \"object\",\n      \"description\": \"Parent project reference\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"Project identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Project name\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Project description\"\n        },\n        \"creationDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Project creation date\"\n        },\n        \"issueTemplateId\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Issue template identifier\"\n        }\n      }\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the creator\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date when the version was created\"\n    },\n    \"issueTemplateId\": {\n      \"type\": \"string\",\n      \"description\": \"Issue template identifier for this version\"\n    },\n    \"currentState\": {\n      \"type\": \"object\",\n      \"description\": \"Current processing state of the version\",\n      \"properties\": {\n        \"committed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the version is committed\"\n        },\n        \"analysisResultsExist\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether analysis results have been uploaded\"\n        },\n        \"hasCustomIssues\"\
  : {\n          \"type\": \"boolean\",\n          \"description\": \"Whether custom issues exist\"\n        },\n        \"auditEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether auditing is enabled\"\n        },\n        \"batchBugSubmissionExists\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether batch bug submissions exist\"\n        }\n      }\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"description\": \"Attribute values assigned to this version\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"attributeDefinitionId\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"description\": \"Attribute definition identifier\"\n          },\n          \"guid\": {\n            \"type\": \"string\",\n            \"description\": \"Attribute GUID\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n          \
  \  \"description\": \"Attribute value\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"guid\": {\n                  \"type\": \"string\"\n                },\n                \"name\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/json-schema/fortify-project-version-schema.json
tags:
- Application Security
- DAST
- DevSecOps
- SAST
- SCA
- Security Testing
- Vulnerability Scanning
title: Fortify Project Version
---
