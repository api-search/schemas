---
description: Schema for a Salesforce Service Cloud Case record representing a customer issue or support request.
layout: schema
name: Salesforce Service Cloud Case
properties_list:
- description: Unique Salesforce record identifier (15 or 18 character)
  name: Id
  type: string
- description: Auto-generated unique case number for display purposes
  name: CaseNumber
  type: string
- description: Brief summary of the customer issue or request
  name: Subject
  type: string
- description: Detailed description of the customer issue
  name: Description
  type: string
- description: Current status in the case lifecycle
  name: Status
  type: string
- description: Priority level indicating urgency of the case
  name: Priority
  type: string
- description: Channel through which the case was created
  name: Origin
  type: string
- description: Classification type of the case
  name: Type
  type: string
- description: Reason the case was created
  name: Reason
  type: string
- description: Salesforce ID of the associated contact
  name: ContactId
  type: string
- description: Salesforce ID of the associated account
  name: AccountId
  type: string
- description: Salesforce ID of the case owner (user or queue)
  name: OwnerId
  type: string
- description: Salesforce ID of the parent case for case hierarchies
  name: ParentId
  type: string
- description: Name supplied by the customer when the case was created via web or email
  name: SuppliedName
  type: string
- description: Email address supplied by the customer
  name: SuppliedEmail
  type: string
- description: Phone number supplied by the customer
  name: SuppliedPhone
  type: string
- description: Whether the case is in a closed status
  name: IsClosed
  type: boolean
- description: Whether the case has been escalated
  name: IsEscalated
  type: boolean
- description: Date and time the case was created
  name: CreatedDate
  type: string
- description: Date and time the case was closed
  name: ClosedDate
  type: string
- description: Date and time the case was last modified
  name: LastModifiedDate
  type: string
- description: Start date for the SLA on this case
  name: SlaStartDate
  type: string
- description: Date the case exited SLA tracking
  name: SlaExitDate
  type: string
- description: Internal case comments
  name: Comments
  type: string
provider_name: Salesforce Service Cloud
provider_slug: salesforce-service-cloud
schema_file: json-schema/salesforce-case-schema.json
slug: salesforce-case
source_filename: salesforce-case-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/service-cloud/case.json\",\n  \"title\": \"Salesforce Service Cloud Case\",\n  \"description\": \"Schema for a Salesforce Service Cloud Case record representing a customer issue or support request.\",\n  \"type\": \"object\",\n  \"required\": [\"Subject\"],\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Salesforce record identifier (15 or 18 character)\",\n      \"pattern\": \"^[a-zA-Z0-9]{15,18}$\"\n    },\n    \"CaseNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-generated unique case number for display purposes\"\n    },\n    \"Subject\": {\n      \"type\": \"string\",\n      \"description\": \"Brief summary of the customer issue or request\",\n      \"maxLength\": 255\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of\
  \ the customer issue\",\n      \"maxLength\": 32000\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status in the case lifecycle\",\n      \"enum\": [\"New\", \"Working\", \"Escalated\", \"Closed\"]\n    },\n    \"Priority\": {\n      \"type\": \"string\",\n      \"description\": \"Priority level indicating urgency of the case\",\n      \"enum\": [\"High\", \"Medium\", \"Low\"]\n    },\n    \"Origin\": {\n      \"type\": \"string\",\n      \"description\": \"Channel through which the case was created\",\n      \"enum\": [\"Phone\", \"Email\", \"Web\", \"Chat\"]\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"Classification type of the case\",\n      \"enum\": [\"Mechanical\", \"Electrical\", \"Electronic\", \"Structural\", \"Other\"]\n    },\n    \"Reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason the case was created\"\n    },\n    \"ContactId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Salesforce ID of the associated contact\",\n      \"pattern\": \"^[a-zA-Z0-9]{15,18}$\"\n    },\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the associated account\",\n      \"pattern\": \"^[a-zA-Z0-9]{15,18}$\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the case owner (user or queue)\",\n      \"pattern\": \"^[a-zA-Z0-9]{15,18}$\"\n    },\n    \"ParentId\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce ID of the parent case for case hierarchies\",\n      \"pattern\": \"^[a-zA-Z0-9]{15,18}$\"\n    },\n    \"SuppliedName\": {\n      \"type\": \"string\",\n      \"description\": \"Name supplied by the customer when the case was created via web or email\",\n      \"maxLength\": 80\n    },\n    \"SuppliedEmail\": {\n      \"type\": \"string\",\n      \"description\": \"Email address supplied by the customer\",\n      \"format\": \"email\",\n      \"maxLength\"\
  : 80\n    },\n    \"SuppliedPhone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number supplied by the customer\",\n      \"maxLength\": 40\n    },\n    \"IsClosed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the case is in a closed status\"\n    },\n    \"IsEscalated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the case has been escalated\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the case was created\"\n    },\n    \"ClosedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the case was closed\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the case was last modified\"\n    },\n    \"SlaStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"\
  description\": \"Start date for the SLA on this case\"\n    },\n    \"SlaExitDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the case exited SLA tracking\"\n    },\n    \"Comments\": {\n      \"type\": \"string\",\n      \"description\": \"Internal case comments\"\n    }\n  },\n  \"$defs\": {\n    \"CaseComment\": {\n      \"type\": \"object\",\n      \"description\": \"A comment on a case record\",\n      \"required\": [\"Body\"],\n      \"properties\": {\n        \"Id\": {\n          \"type\": \"string\",\n          \"description\": \"Comment record ID\"\n        },\n        \"ParentId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the parent case\"\n        },\n        \"Body\": {\n          \"type\": \"string\",\n          \"description\": \"Text body of the comment\"\n        },\n        \"IsPublished\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the comment is visible\
  \ to the customer\"\n        },\n        \"CreatedDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the comment was created\"\n        },\n        \"CreatedById\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the user who created the comment\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-service-cloud/refs/heads/main/json-schema/salesforce-case-schema.json
tags:
- Case Management
- CRM
- Customer Service
- Help Desk
- Support
- Ticketing
title: Salesforce Service Cloud Case
---
