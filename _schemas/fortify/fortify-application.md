---
description: Represents an application in the Fortify platform that is subject to security testing. An application contains one or more releases and may be organized with microservices. Applications are the primary organizational unit for managing security assessments.
layout: schema
name: Fortify Application
properties_list:
- description: Unique identifier of the application
  name: applicationId
  type: integer
- description: Name of the application
  name: applicationName
  type: string
- description: Description of the application and its purpose
  name: applicationDescription
  type: string
- description: Date and time when the application was created in ISO 8601 format
  name: applicationCreatedDate
  type: string
- description: Business criticality classification indicating the importance of the application
  name: businessCriticalityType
  type: string
- description: Current software development lifecycle status of the application
  name: sdlcStatusType
  type: string
- description: Comma-separated list of email addresses for notifications
  name: emailList
  type: string
- description: Whether the application has microservices configured
  name: hasMicroservices
  type: boolean
- description: Custom attributes assigned to the application
  name: attributes
  type: array
- description: Releases associated with this application
  name: releases
  type: array
provider_name: Fortify
provider_slug: fortify
schema_file: json-schema/fortify-application-schema.json
slug: fortify-application
source_filename: fortify-application-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/fortify/json-schema/fortify-application-schema.json\",\n  \"title\": \"Fortify Application\",\n  \"description\": \"Represents an application in the Fortify platform that is subject to security testing. An application contains one or more releases and may be organized with microservices. Applications are the primary organizational unit for managing security assessments.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"applicationName\"\n  ],\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"Unique identifier of the application\"\n    },\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the application\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"applicationDescription\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Description of the application and its purpose\"\n    },\n    \"applicationCreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the application was created in ISO 8601 format\"\n    },\n    \"businessCriticalityType\": {\n      \"type\": \"string\",\n      \"description\": \"Business criticality classification indicating the importance of the application\",\n      \"enum\": [\n        \"High\",\n        \"Medium\",\n        \"Low\"\n      ]\n    },\n    \"sdlcStatusType\": {\n      \"type\": \"string\",\n      \"description\": \"Current software development lifecycle status of the application\",\n      \"enum\": [\n        \"Development\",\n        \"QA\",\n        \"Production\",\n        \"Retired\"\n      ]\n    },\n    \"emailList\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of email addresses for notifications\"\n    },\n    \"hasMicroservices\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether the application has microservices configured\",\n      \"default\": false\n    },\n    \"attributes\": {\n      \"type\": \"array\",\n      \"description\": \"Custom attributes assigned to the application\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"format\": \"int32\",\n            \"description\": \"Attribute definition identifier\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Attribute name\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"Attribute value\"\n          }\n        }\n      }\n    },\n    \"releases\": {\n      \"type\": \"array\",\n      \"description\": \"Releases associated with this application\",\n      \"items\": {\n        \"$ref\": \"fortify-release-schema.json\"\n      }\n    }\n  },\n  \"additionalProperties\"\
  : true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fortify/refs/heads/main/json-schema/fortify-application-schema.json
tags:
- Application Security
- DAST
- DevSecOps
- SAST
- SCA
- Security Testing
- Vulnerability Scanning
title: Fortify Application
---
