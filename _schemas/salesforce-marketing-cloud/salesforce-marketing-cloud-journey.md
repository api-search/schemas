---
description: Represents a customer journey in Marketing Cloud. A journey defines an automated workflow that guides contacts through a series of marketing interactions across channels.
layout: schema
name: Journey
properties_list:
- description: System-generated unique identifier for the journey
  name: id
  type: string
- description: Customer-defined unique key for the journey
  name: key
  type: string
- description: Display name of the journey
  name: name
  type: string
- description: Description of the journey purpose
  name: description
  type: string
- description: Current version number of the journey
  name: version
  type: integer
- description: Current status of the journey
  name: status
  type: string
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
- description: Version of the Journey Builder API used
  name: workflowApiVersion
  type: number
- description: Entry triggers that inject contacts into the journey
  name: triggers
  type: array
- description: Activities that contacts pass through in the journey
  name: activities
  type: array
- description: Goal criteria that measure journey success
  name: goals
  type: array
- description: Exit criteria that remove contacts from the journey
  name: exits
  type: array
- description: Runtime statistics for the journey
  name: stats
  type: object
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-journey-schema.json
slug: salesforce-marketing-cloud-journey
source_filename: salesforce-marketing-cloud-journey-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Journey\",\n  \"type\": \"object\",\n  \"description\": \"Represents a customer journey in Marketing Cloud. A journey defines an automated workflow that guides contacts through a series of marketing interactions across channels.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"System-generated unique identifier for the journey\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Customer-defined unique key for the journey\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the journey\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the journey purpose\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Current version number of the journey\"\n    },\n    \"status\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Current status of the journey\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\"\n    },\n    \"workflowApiVersion\": {\n      \"type\": \"number\",\n      \"description\": \"Version of the Journey Builder API used\"\n    },\n    \"triggers\": {\n      \"type\": \"array\",\n      \"description\": \"Entry triggers that inject contacts into the journey\"\n    },\n    \"activities\": {\n      \"type\": \"array\",\n      \"description\": \"Activities that contacts pass through in the journey\"\n    },\n    \"goals\": {\n      \"type\": \"array\",\n      \"description\": \"Goal criteria that measure journey success\"\n    },\n    \"exits\": {\n      \"type\": \"array\",\n      \"description\": \"Exit criteria that remove contacts from the journey\"\n    },\n    \"stats\": {\n      \"type\": \"object\",\n      \"description\": \"Runtime statistics for the journey\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-journey-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: Journey
---
