---
description: Represents an in-flight deployment package associated with an Appian application. Contains metadata about the package contents and status.
layout: schema
name: Package
properties_list:
- description: The name of the deployment package.
  name: name
  type: string
- description: A description of the deployment package.
  name: description
  type: string
- description: The unique identifier for the package. This UUID can be used with the Deployment REST API for exports and deployments.
  name: uuid
  type: string
- description: The number of design objects included in the package.
  name: objectCount
  type: integer
- description: The number of database scripts included in the package.
  name: databaseScriptCount
  type: integer
- description: The number of plug-ins included in the package.
  name: pluginCount
  type: integer
- description: The UUID of the data source associated with the package, if applicable.
  name: datasourceUuid
  type: string
- description: Indicates whether the package includes an import customization file.
  name: hasCustomizationFile
  type: boolean
- description: The timestamp when the package was created.
  name: createdTimestamp
  type: string
- description: The timestamp when the package was last modified. Packages are sorted by this field in descending order.
  name: lastModifiedTimestamp
  type: string
- description: A link to an external ticket or change request associated with this package.
  name: ticketLink
  type: string
provider_name: Appian
provider_slug: appian
schema_file: json-schema/application-package-details-package-schema.json
slug: application-package-details-package
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/application-package-details-package-schema.json\",\n  \"title\": \"Package\",\n  \"description\": \"Represents an in-flight deployment package associated with an Appian application. Contains metadata about the package contents and status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the deployment package.\",\n      \"example\": \"CR-176543 Add reports dashboard\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the deployment package.\",\n      \"example\": \"Updates the executive summary view with new reports.\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the package. This UUID can\
  \ be used with the Deployment REST API for exports and deployments.\",\n      \"example\": \"d243b14c-3ba5-41c3-9f51-76da51beb8f5\"\n    },\n    \"objectCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of design objects included in the package.\",\n      \"minimum\": 0,\n      \"example\": 12\n    },\n    \"databaseScriptCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of database scripts included in the package.\",\n      \"minimum\": 0,\n      \"example\": 2\n    },\n    \"pluginCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of plug-ins included in the package.\",\n      \"minimum\": 0,\n      \"example\": 1\n    },\n    \"datasourceUuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The UUID of the data source associated with the package, if applicable.\"\n    },\n    \"hasCustomizationFile\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates\
  \ whether the package includes an import customization file.\",\n      \"example\": true\n    },\n    \"createdTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the package was created.\"\n    },\n    \"lastModifiedTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the package was last modified. Packages are sorted by this field in descending order.\"\n    },\n    \"ticketLink\": {\n      \"type\": \"string\",\n      \"description\": \"A link to an external ticket or change request associated with this package.\",\n      \"example\": \"https://jira.example.com/browse/CR-176543\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"uuid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/json-schema/application-package-details-package-schema.json
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
title: Package
---
