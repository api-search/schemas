---
description: Represents a case, which is a customer issue or problem. Cases are used to track and manage customer support inquiries, complaints, and service requests. Cases can be associated with accounts, contacts, and assets.
layout: schema
name: Salesforce Case
properties_list:
- description: Unique 18-character Salesforce record identifier
  name: Id
  type: string
- description: Indicates whether the record has been moved to the Recycle Bin
  name: IsDeleted
  type: boolean
- description: If deleted as result of a merge, ID of the master record
  name: MasterRecordId
  type:
  - string
  - 'null'
- description: Auto-number identifier for the case
  name: CaseNumber
  type: string
- description: ID of the associated Contact
  name: ContactId
  type:
  - string
  - 'null'
- description: ID of the associated Account
  name: AccountId
  type:
  - string
  - 'null'
- description: ID of the associated Asset
  name: AssetId
  type:
  - string
  - 'null'
- description: ID of the parent case (for case hierarchies)
  name: ParentId
  type:
  - string
  - 'null'
- description: Name of the contact supplied during case creation via Web-to-Case
  name: SuppliedName
  type:
  - string
  - 'null'
- description: Email address supplied during case creation
  name: SuppliedEmail
  type:
  - string
  - 'null'
- description: Phone number supplied during case creation
  name: SuppliedPhone
  type:
  - string
  - 'null'
- description: Company name supplied during case creation
  name: SuppliedCompany
  type:
  - string
  - 'null'
- description: Type of case
  name: Type
  type:
  - string
  - 'null'
- description: Status of the case
  name: Status
  type: string
- description: Reason the case was created
  name: Reason
  type:
  - string
  - 'null'
- description: Source of the case
  name: Origin
  type:
  - string
  - 'null'
- description: Subject of the case
  name: Subject
  type:
  - string
  - 'null'
- description: Priority of the case
  name: Priority
  type:
  - string
  - 'null'
- description: Full description of the case
  name: Description
  type:
  - string
  - 'null'
- description: Indicates whether the case is closed
  name: IsClosed
  type: boolean
- description: Date and time when the case was closed
  name: ClosedDate
  type:
  - string
  - 'null'
- description: Indicates whether the case has been escalated
  name: IsEscalated
  type: boolean
- description: ID of the user or queue that owns the case
  name: OwnerId
  type: string
- description: Date and time when this record was created
  name: CreatedDate
  type: string
- description: ID of the user who created this record
  name: CreatedById
  type: string
- description: Date and time when this record was last modified
  name: LastModifiedDate
  type: string
- description: ID of the user who last modified this record
  name: LastModifiedById
  type: string
- description: ''
  name: SystemModstamp
  type: string
- description: Phone number of the associated contact
  name: ContactPhone
  type:
  - string
  - 'null'
- description: Mobile phone number of the associated contact
  name: ContactMobile
  type:
  - string
  - 'null'
- description: Email of the associated contact
  name: ContactEmail
  type:
  - string
  - 'null'
- description: Fax of the associated contact
  name: ContactFax
  type:
  - string
  - 'null'
- description: Internal comments associated with this case
  name: Comments
  type:
  - string
  - 'null'
- description: ''
  name: LastViewedDate
  type:
  - string
  - 'null'
- description: ''
  name: LastReferencedDate
  type:
  - string
  - 'null'
- description: ''
  name: attributes
  type: object
provider_name: Salesforce Sales Cloud
provider_slug: salesforce-sales-cloud
schema_file: json-schema/salesforce-sales-cloud-case-schema.json
slug: salesforce-sales-cloud-case
source_filename: salesforce-sales-cloud-case-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/sales-cloud/case.json\",\n  \"title\": \"Salesforce Case\",\n  \"description\": \"Represents a case, which is a customer issue or problem. Cases are used to track and manage customer support inquiries, complaints, and service requests. Cases can be associated with accounts, contacts, and assets.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce record identifier\",\n      \"pattern\": \"^[a-zA-Z0-9]{18}$\",\n      \"readOnly\": true\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the record has been moved to the Recycle Bin\",\n      \"readOnly\": true\n    },\n    \"MasterRecordId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"If deleted as result of a merge, ID of the master\
  \ record\",\n      \"readOnly\": true\n    },\n    \"CaseNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-number identifier for the case\",\n      \"readOnly\": true\n    },\n    \"ContactId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the associated Contact\"\n    },\n    \"AccountId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the associated Account\"\n    },\n    \"AssetId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the associated Asset\"\n    },\n    \"ParentId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the parent case (for case hierarchies)\"\n    },\n    \"SuppliedName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name of the contact supplied during case creation via Web-to-Case\",\n      \"maxLength\": 80\n    },\n    \"SuppliedEmail\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\"\
  : \"Email address supplied during case creation\",\n      \"format\": \"email\",\n      \"maxLength\": 80\n    },\n    \"SuppliedPhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Phone number supplied during case creation\",\n      \"maxLength\": 40\n    },\n    \"SuppliedCompany\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Company name supplied during case creation\",\n      \"maxLength\": 80\n    },\n    \"Type\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Type of case\",\n      \"enum\": [null, \"Mechanical\", \"Electrical\", \"Electronic\", \"Structural\", \"Other\"]\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the case\",\n      \"enum\": [\"New\", \"Working\", \"Escalated\", \"Closed\"]\n    },\n    \"Reason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Reason the case was created\",\n      \"enum\": [null, \"Installation\", \"\
  Equipment Complexity\", \"Performance\", \"Breakdown\", \"Equipment Design\", \"Feedback\", \"Other\"]\n    },\n    \"Origin\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Source of the case\",\n      \"enum\": [null, \"Phone\", \"Email\", \"Web\"]\n    },\n    \"Subject\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Subject of the case\",\n      \"maxLength\": 255\n    },\n    \"Priority\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Priority of the case\",\n      \"enum\": [null, \"High\", \"Medium\", \"Low\"]\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Full description of the case\"\n    },\n    \"IsClosed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the case is closed\",\n      \"readOnly\": true\n    },\n    \"ClosedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Date and time when the case was closed\",\n      \"readOnly\": true\n    },\n    \"IsEscalated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the case has been escalated\",\n      \"default\": false\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user or queue that owns the case\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was created\",\n      \"readOnly\": true\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created this record\",\n      \"readOnly\": true\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was last modified\",\n      \"readOnly\": true\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"ID of the user who last modified this record\",\n      \"readOnly\": true\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"ContactPhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Phone number of the associated contact\",\n      \"readOnly\": true\n    },\n    \"ContactMobile\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Mobile phone number of the associated contact\",\n      \"readOnly\": true\n    },\n    \"ContactEmail\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Email of the associated contact\",\n      \"readOnly\": true\n    },\n    \"ContactFax\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Fax of the associated contact\",\n      \"readOnly\": true\n    },\n    \"Comments\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Internal comments associated with this case\"\
  \n    },\n    \"LastViewedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"LastReferencedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Case\"\n        },\n        \"url\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"Status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/json-schema/salesforce-sales-cloud-case-schema.json
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
title: Salesforce Case
---
