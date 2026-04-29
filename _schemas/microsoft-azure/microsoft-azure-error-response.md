---
description: The common error response schema for all Azure Resource Manager APIs. This follows the Azure REST API guidelines for error handling, providing structured error information including error codes, messages, targets, and nested details for comprehensive error diagnostics.
layout: schema
name: Azure Error Response
properties_list:
- description: ''
  name: error
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/microsoft-azure-error-response-schema.json
slug: microsoft-azure-error-response
source_filename: microsoft-azure-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-azure/error-response\",\n  \"title\": \"Azure Error Response\",\n  \"description\": \"The common error response schema for all Azure Resource Manager APIs. This follows the Azure REST API guidelines for error handling, providing structured error information including error codes, messages, targets, and nested details for comprehensive error diagnostics.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"$ref\": \"#/$defs/ErrorDetail\"\n    }\n  },\n  \"$defs\": {\n    \"ErrorDetail\": {\n      \"type\": \"object\",\n      \"description\": \"The error detail.\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"The error code. This is a machine-readable identifier for the error that can be used for programmatic error handling.\",\n          \"readOnly\": true,\n          \"examples\"\
  : [\n            \"ResourceNotFound\",\n            \"InvalidRequestContent\",\n            \"AuthorizationFailed\",\n            \"ResourceGroupNotFound\",\n            \"SubscriptionNotFound\",\n            \"MissingSubscriptionRegistration\",\n            \"InvalidParameter\",\n            \"ConflictError\",\n            \"OperationNotAllowed\"\n          ]\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"The error message. This is a human-readable description of the error intended for display in a user interface.\",\n          \"readOnly\": true\n        },\n        \"target\": {\n          \"type\": \"string\",\n          \"description\": \"The error target. This identifies the specific element (property name, path, etc.) that is the source of the error.\",\n          \"readOnly\": true\n        },\n        \"details\": {\n          \"type\": \"array\",\n          \"description\": \"The error details. A list of additional error objects\
  \ providing more granular information about the error.\",\n          \"readOnly\": true,\n          \"items\": {\n            \"$ref\": \"#/$defs/ErrorDetail\"\n          }\n        },\n        \"additionalInfo\": {\n          \"type\": \"array\",\n          \"description\": \"The error additional info. Additional structured data about the error for programmatic consumption.\",\n          \"readOnly\": true,\n          \"items\": {\n            \"$ref\": \"#/$defs/ErrorAdditionalInfo\"\n          }\n        }\n      }\n    },\n    \"ErrorAdditionalInfo\": {\n      \"type\": \"object\",\n      \"description\": \"The resource management error additional info.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The additional info type. Identifies the schema of the info property.\",\n          \"readOnly\": true\n        },\n        \"info\": {\n          \"type\": \"object\",\n          \"description\": \"The additional info. Contains\
  \ structured data specific to the error additional info type.\",\n          \"readOnly\": true\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/microsoft-azure-error-response-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Azure Error Response
---
