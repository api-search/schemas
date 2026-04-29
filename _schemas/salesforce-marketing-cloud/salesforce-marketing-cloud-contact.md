---
description: Represents a contact in Marketing Cloud. A contact is an individual who interacts with marketing campaigns across channels.
layout: schema
name: Contact
properties_list:
- description: Unique identifier for the contact. This value is used across all Marketing Cloud channels and applications.
  name: contactKey
  type: string
- description: System-generated unique numeric identifier
  name: contactID
  type: integer
- description: Current status of the contact
  name: contactStatus
  type: string
- description: Date and time the contact was created
  name: createdDate
  type: string
- description: Date and time the contact was last modified
  name: modifiedDate
  type: string
- description: Collection of attribute sets associated with the contact
  name: attributeSets
  type: array
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
schema_file: json-schema/salesforce-marketing-cloud-contact-schema.json
slug: salesforce-marketing-cloud-contact
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Contact\",\n  \"type\": \"object\",\n  \"description\": \"Represents a contact in Marketing Cloud. A contact is an individual who interacts with marketing campaigns across channels.\",\n  \"properties\": {\n    \"contactKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the contact. This value is used across all Marketing Cloud channels and applications.\"\n    },\n    \"contactID\": {\n      \"type\": \"integer\",\n      \"description\": \"System-generated unique numeric identifier\"\n    },\n    \"contactStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the contact\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the contact was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time the contact was last modified\"\
  \n    },\n    \"attributeSets\": {\n      \"type\": \"array\",\n      \"description\": \"Collection of attribute sets associated with the contact\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/json-schema/salesforce-marketing-cloud-contact-schema.json
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
title: Contact
---
