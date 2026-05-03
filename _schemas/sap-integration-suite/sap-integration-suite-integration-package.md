---
description: Schema for an SAP Cloud Integration package containing integration artifacts
layout: schema
name: SAP Integration Package
properties_list:
- description: Unique identifier of the integration package
  name: Id
  type: string
- description: Display name of the integration package
  name: Name
  type: string
- description: Detailed description of the package
  name: Description
  type: string
- description: Short description of the package
  name: ShortText
  type: string
- description: Package version in semantic versioning format
  name: Version
  type: string
- description: Vendor or publisher of the package
  name: Vendor
  type: string
- description: Edit mode for the package
  name: Mode
  type: string
- description: Supported runtime platform
  name: SupportedPlatform
  type: string
- description: ISO 8601 creation timestamp
  name: CreationDate
  type: string
- description: ISO 8601 last modification timestamp
  name: ModifiedDate
  type: string
provider_name: SAP Integration Suite
provider_slug: sap-integration-suite
schema_file: json-schema/sap-integration-suite-integration-package-schema.json
slug: sap-integration-suite-integration-package
source_filename: sap-integration-suite-integration-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sap-integration-suite/json-schema/sap-integration-suite-integration-package-schema.json\",\n  \"title\": \"SAP Integration Package\",\n  \"description\": \"Schema for an SAP Cloud Integration package containing integration artifacts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the integration package\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the integration package\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the package\"\n    },\n    \"ShortText\": {\n      \"type\": \"string\",\n      \"description\": \"Short description of the package\",\n      \"maxLength\": 140\n    },\n    \"Version\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Package version in semantic versioning format\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.\\\\d+$\"\n    },\n    \"Vendor\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor or publisher of the package\"\n    },\n    \"Mode\": {\n      \"type\": \"string\",\n      \"description\": \"Edit mode for the package\",\n      \"enum\": [\"EDIT_ALLOWED\", \"READONLY\"]\n    },\n    \"SupportedPlatform\": {\n      \"type\": \"string\",\n      \"description\": \"Supported runtime platform\",\n      \"enum\": [\"SAP Cloud Integration\", \"SAP Integration Suite\"]\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 creation timestamp\",\n      \"format\": \"date-time\"\n    },\n    \"ModifiedDate\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 last modification timestamp\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"Id\", \"Name\", \"Version\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/json-schema/sap-integration-suite-integration-package-schema.json
tags:
- API Management
- Cloud Integration
- Enterprise Integration
- Event Mesh
- iPaaS
- SAP
- SAP BTP
title: SAP Integration Package
---
