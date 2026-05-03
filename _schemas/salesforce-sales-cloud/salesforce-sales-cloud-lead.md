---
description: Represents a prospect or lead. A lead is a person who has expressed interest in your company or products but has not yet been qualified as a potential buyer. After qualification, leads can be converted to accounts, contacts, and opportunities.
layout: schema
name: Salesforce Lead
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
- description: Last name of the lead
  name: LastName
  type: string
- description: First name of the lead
  name: FirstName
  type:
  - string
  - 'null'
- description: Honorific abbreviation or title
  name: Salutation
  type:
  - string
  - 'null'
- description: Concatenation of FirstName, MiddleName, LastName, and Suffix
  name: Name
  type: string
- description: Middle name of the lead
  name: MiddleName
  type:
  - string
  - 'null'
- description: Name suffix of the lead
  name: Suffix
  type:
  - string
  - 'null'
- description: Title of the lead, such as CEO or Vice President
  name: Title
  type:
  - string
  - 'null'
- description: Name of the company associated with the lead
  name: Company
  type: string
- description: Street address for the lead
  name: Street
  type:
  - string
  - 'null'
- description: City for the lead's address
  name: City
  type:
  - string
  - 'null'
- description: State or province for the lead's address
  name: State
  type:
  - string
  - 'null'
- description: Postal code for the lead's address
  name: PostalCode
  type:
  - string
  - 'null'
- description: Country for the lead's address
  name: Country
  type:
  - string
  - 'null'
- description: Latitude of the lead's address
  name: Latitude
  type:
  - number
  - 'null'
- description: Longitude of the lead's address
  name: Longitude
  type:
  - number
  - 'null'
- description: Phone number for the lead
  name: Phone
  type:
  - string
  - 'null'
- description: Mobile phone number for the lead
  name: MobilePhone
  type:
  - string
  - 'null'
- description: Fax number for the lead
  name: Fax
  type:
  - string
  - 'null'
- description: Email address for the lead
  name: Email
  type:
  - string
  - 'null'
- description: Website for the lead
  name: Website
  type:
  - string
  - 'null'
- description: Text description of the lead
  name: Description
  type:
  - string
  - 'null'
- description: Source from which the lead was obtained
  name: LeadSource
  type:
  - string
  - 'null'
- description: Status of the lead (e.g., Open, Contacted, Qualified)
  name: Status
  type: string
- description: Industry associated with the lead
  name: Industry
  type:
  - string
  - 'null'
- description: Rating for the lead
  name: Rating
  type:
  - string
  - 'null'
- description: Annual revenue of the lead's company
  name: AnnualRevenue
  type:
  - number
  - 'null'
- description: Number of employees at the lead's company
  name: NumberOfEmployees
  type:
  - integer
  - 'null'
- description: ID of the user who owns this lead
  name: OwnerId
  type: string
- description: Indicates whether the lead has been converted (true) or not (false)
  name: IsConverted
  type: boolean
- description: Date when the lead was converted
  name: ConvertedDate
  type:
  - string
  - 'null'
- description: Object reference ID of the account into which the lead converted
  name: ConvertedAccountId
  type:
  - string
  - 'null'
- description: Object reference ID of the contact into which the lead converted
  name: ConvertedContactId
  type:
  - string
  - 'null'
- description: Object reference ID of the opportunity created during lead conversion
  name: ConvertedOpportunityId
  type:
  - string
  - 'null'
- description: Indicates whether the lead has been read by the owner
  name: IsUnreadByOwner
  type: boolean
- description: Indicates the lead does not wish to receive email
  name: HasOptedOutOfEmail
  type: boolean
- description: Indicates the lead does not wish to be called
  name: DoNotCall
  type: boolean
- description: Indicates the lead does not wish to receive faxes
  name: HasOptedOutOfFax
  type: boolean
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
- description: ''
  name: LastActivityDate
  type:
  - string
  - 'null'
- description: ''
  name: Jigsaw
  type:
  - string
  - 'null'
- description: ''
  name: JigsawContactId
  type:
  - string
  - 'null'
- description: ''
  name: CleanStatus
  type:
  - string
  - 'null'
- description: D-U-N-S number for the lead's company
  name: CompanyDunsNumber
  type:
  - string
  - 'null'
- description: ID of the related individual record for data privacy
  name: IndividualId
  type:
  - string
  - 'null'
- description: ''
  name: attributes
  type: object
provider_name: Salesforce Sales Cloud
provider_slug: salesforce-sales-cloud
schema_file: json-schema/salesforce-sales-cloud-lead-schema.json
slug: salesforce-sales-cloud-lead
source_filename: salesforce-sales-cloud-lead-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/sales-cloud/lead.json\",\n  \"title\": \"Salesforce Lead\",\n  \"description\": \"Represents a prospect or lead. A lead is a person who has expressed interest in your company or products but has not yet been qualified as a potential buyer. After qualification, leads can be converted to accounts, contacts, and opportunities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce record identifier\",\n      \"pattern\": \"^[a-zA-Z0-9]{18}$\",\n      \"readOnly\": true\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the record has been moved to the Recycle Bin\",\n      \"readOnly\": true\n    },\n    \"MasterRecordId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"If deleted as result\
  \ of a merge, ID of the master record\",\n      \"readOnly\": true\n    },\n    \"LastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the lead\",\n      \"maxLength\": 80\n    },\n    \"FirstName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"First name of the lead\",\n      \"maxLength\": 40\n    },\n    \"Salutation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Honorific abbreviation or title\",\n      \"enum\": [null, \"Mr.\", \"Ms.\", \"Mrs.\", \"Dr.\", \"Prof.\"]\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Concatenation of FirstName, MiddleName, LastName, and Suffix\",\n      \"readOnly\": true\n    },\n    \"MiddleName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Middle name of the lead\",\n      \"maxLength\": 40\n    },\n    \"Suffix\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name suffix of the lead\",\n   \
  \   \"maxLength\": 40\n    },\n    \"Title\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Title of the lead, such as CEO or Vice President\",\n      \"maxLength\": 128\n    },\n    \"Company\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the company associated with the lead\",\n      \"maxLength\": 255\n    },\n    \"Street\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Street address for the lead\"\n    },\n    \"City\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"City for the lead's address\",\n      \"maxLength\": 40\n    },\n    \"State\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"State or province for the lead's address\",\n      \"maxLength\": 80\n    },\n    \"PostalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Postal code for the lead's address\",\n      \"maxLength\": 20\n    },\n    \"Country\": {\n      \"type\": [\"string\"\
  , \"null\"],\n      \"description\": \"Country for the lead's address\",\n      \"maxLength\": 80\n    },\n    \"Latitude\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Latitude of the lead's address\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"Longitude\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Longitude of the lead's address\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    },\n    \"Phone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Phone number for the lead\",\n      \"maxLength\": 40\n    },\n    \"MobilePhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Mobile phone number for the lead\",\n      \"maxLength\": 40\n    },\n    \"Fax\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Fax number for the lead\",\n      \"maxLength\": 40\n    },\n    \"Email\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"\
  Email address for the lead\",\n      \"format\": \"email\",\n      \"maxLength\": 80\n    },\n    \"Website\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Website for the lead\",\n      \"format\": \"uri\",\n      \"maxLength\": 255\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Text description of the lead\"\n    },\n    \"LeadSource\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Source from which the lead was obtained\",\n      \"enum\": [null, \"Web\", \"Phone Inquiry\", \"Partner Referral\", \"Purchased List\", \"Other\"]\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the lead (e.g., Open, Contacted, Qualified)\",\n      \"enum\": [\"Open - Not Contacted\", \"Working - Contacted\", \"Closed - Converted\", \"Closed - Not Converted\"]\n    },\n    \"Industry\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Industry associated\
  \ with the lead\",\n      \"enum\": [\n        null,\n        \"Agriculture\",\n        \"Apparel\",\n        \"Banking\",\n        \"Biotechnology\",\n        \"Chemicals\",\n        \"Communications\",\n        \"Construction\",\n        \"Consulting\",\n        \"Education\",\n        \"Electronics\",\n        \"Energy\",\n        \"Engineering\",\n        \"Entertainment\",\n        \"Environmental\",\n        \"Finance\",\n        \"Food & Beverage\",\n        \"Government\",\n        \"Healthcare\",\n        \"Hospitality\",\n        \"Insurance\",\n        \"Machinery\",\n        \"Manufacturing\",\n        \"Media\",\n        \"Not For Profit\",\n        \"Recreation\",\n        \"Retail\",\n        \"Shipping\",\n        \"Technology\",\n        \"Telecommunications\",\n        \"Transportation\",\n        \"Utilities\",\n        \"Other\"\n      ]\n    },\n    \"Rating\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Rating for the lead\",\n      \"enum\"\
  : [null, \"Hot\", \"Warm\", \"Cold\"]\n    },\n    \"AnnualRevenue\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Annual revenue of the lead's company\"\n    },\n    \"NumberOfEmployees\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Number of employees at the lead's company\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who owns this lead\"\n    },\n    \"IsConverted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the lead has been converted (true) or not (false)\",\n      \"readOnly\": true\n    },\n    \"ConvertedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date when the lead was converted\",\n      \"readOnly\": true\n    },\n    \"ConvertedAccountId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Object reference ID of the account into which the lead converted\",\n\
  \      \"readOnly\": true\n    },\n    \"ConvertedContactId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Object reference ID of the contact into which the lead converted\",\n      \"readOnly\": true\n    },\n    \"ConvertedOpportunityId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Object reference ID of the opportunity created during lead conversion\",\n      \"readOnly\": true\n    },\n    \"IsUnreadByOwner\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the lead has been read by the owner\"\n    },\n    \"HasOptedOutOfEmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates the lead does not wish to receive email\",\n      \"default\": false\n    },\n    \"DoNotCall\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates the lead does not wish to be called\",\n      \"default\": false\n    },\n    \"HasOptedOutOfFax\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Indicates the lead does not wish to receive faxes\",\n      \"default\": false\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was created\",\n      \"readOnly\": true\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created this record\",\n      \"readOnly\": true\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was last modified\",\n      \"readOnly\": true\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified this record\",\n      \"readOnly\": true\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"LastActivityDate\": {\n      \"type\": [\"string\", \"null\"\
  ],\n      \"format\": \"date\",\n      \"readOnly\": true\n    },\n    \"Jigsaw\": {\n      \"type\": [\"string\", \"null\"],\n      \"maxLength\": 20\n    },\n    \"JigsawContactId\": {\n      \"type\": [\"string\", \"null\"],\n      \"readOnly\": true\n    },\n    \"CleanStatus\": {\n      \"type\": [\"string\", \"null\"],\n      \"enum\": [null, \"Matched\", \"Different\", \"Acknowledged\", \"NotFound\", \"Inactive\", \"Pending\", \"SelectMatch\", \"Skipped\"]\n    },\n    \"CompanyDunsNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"D-U-N-S number for the lead's company\",\n      \"maxLength\": 9\n    },\n    \"IndividualId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the related individual record for data privacy\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Lead\"\n        },\n        \"url\": {\n   \
  \       \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"LastName\", \"Company\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/json-schema/salesforce-sales-cloud-lead-schema.json
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
title: Salesforce Lead
---
