---
description: Represents a contact, which is a person associated with an account. Contacts are one of the core objects in Salesforce Sales Cloud for managing relationships with individuals at customer organizations.
layout: schema
name: Salesforce Contact
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
- description: ID of the account that is the parent of this contact
  name: AccountId
  type:
  - string
  - 'null'
- description: Last name of the contact
  name: LastName
  type: string
- description: First name of the contact
  name: FirstName
  type:
  - string
  - 'null'
- description: Honorific abbreviation or title of the contact
  name: Salutation
  type:
  - string
  - 'null'
- description: Concatenation of FirstName, MiddleName, LastName, and Suffix
  name: Name
  type: string
- description: Middle name of the contact
  name: MiddleName
  type:
  - string
  - 'null'
- description: Name suffix of the contact
  name: Suffix
  type:
  - string
  - 'null'
- description: Street address for the other address
  name: OtherStreet
  type:
  - string
  - 'null'
- description: City for the other address
  name: OtherCity
  type:
  - string
  - 'null'
- description: State for the other address
  name: OtherState
  type:
  - string
  - 'null'
- description: Postal code for the other address
  name: OtherPostalCode
  type:
  - string
  - 'null'
- description: Country for the other address
  name: OtherCountry
  type:
  - string
  - 'null'
- description: Latitude for the other address
  name: OtherLatitude
  type:
  - number
  - 'null'
- description: Longitude for the other address
  name: OtherLongitude
  type:
  - number
  - 'null'
- description: Street address for the mailing address
  name: MailingStreet
  type:
  - string
  - 'null'
- description: City for the mailing address
  name: MailingCity
  type:
  - string
  - 'null'
- description: State for the mailing address
  name: MailingState
  type:
  - string
  - 'null'
- description: Postal code for the mailing address
  name: MailingPostalCode
  type:
  - string
  - 'null'
- description: Country for the mailing address
  name: MailingCountry
  type:
  - string
  - 'null'
- description: Latitude for the mailing address
  name: MailingLatitude
  type:
  - number
  - 'null'
- description: Longitude for the mailing address
  name: MailingLongitude
  type:
  - number
  - 'null'
- description: Phone number for the contact
  name: Phone
  type:
  - string
  - 'null'
- description: Fax number for the contact
  name: Fax
  type:
  - string
  - 'null'
- description: Contact's mobile phone number
  name: MobilePhone
  type:
  - string
  - 'null'
- description: Home phone number for the contact
  name: HomePhone
  type:
  - string
  - 'null'
- description: Other phone number for the contact
  name: OtherPhone
  type:
  - string
  - 'null'
- description: Phone number for the contact's assistant
  name: AssistantPhone
  type:
  - string
  - 'null'
- description: ID of the contact that this contact reports to
  name: ReportsToId
  type:
  - string
  - 'null'
- description: Email address for the contact
  name: Email
  type:
  - string
  - 'null'
- description: Title of the contact, such as CEO or Vice President
  name: Title
  type:
  - string
  - 'null'
- description: Department of the contact
  name: Department
  type:
  - string
  - 'null'
- description: Name of the assistant
  name: AssistantName
  type:
  - string
  - 'null'
- description: Source from which the contact was obtained
  name: LeadSource
  type:
  - string
  - 'null'
- description: Birthdate for the contact
  name: Birthdate
  type:
  - string
  - 'null'
- description: Text description of the contact
  name: Description
  type:
  - string
  - 'null'
- description: ID of the owner of the account associated with this contact
  name: OwnerId
  type: string
- description: Indicates whether the contact has opted out of email (true) or not (false)
  name: HasOptedOutOfEmail
  type: boolean
- description: Indicates whether the contact has opted out of fax (true) or not (false)
  name: HasOptedOutOfFax
  type: boolean
- description: Indicates that the contact does not want to be called
  name: DoNotCall
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
- description: Date and time when this record was last modified by a user or process
  name: SystemModstamp
  type: string
- description: Most recent activity date
  name: LastActivityDate
  type:
  - string
  - 'null'
- description: Last date the contact was requested via a customer update
  name: LastCURequestDate
  type:
  - string
  - 'null'
- description: Last date the contact was updated via a customer update
  name: LastCUUpdateDate
  type:
  - string
  - 'null'
- description: If bounced, the reason for the bounce
  name: EmailBouncedReason
  type:
  - string
  - 'null'
- description: If bounced, the date and time the bounce occurred
  name: EmailBouncedDate
  type:
  - string
  - 'null'
- description: References the ID of a contact in Data.com
  name: Jigsaw
  type:
  - string
  - 'null'
- description: References a contact in Data.com
  name: JigsawContactId
  type:
  - string
  - 'null'
- description: Indicates the record's clean status as compared with Data.com
  name: CleanStatus
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
schema_file: json-schema/salesforce-sales-cloud-contact-schema.json
slug: salesforce-sales-cloud-contact
source_filename: salesforce-sales-cloud-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/sales-cloud/contact.json\",\n  \"title\": \"Salesforce Contact\",\n  \"description\": \"Represents a contact, which is a person associated with an account. Contacts are one of the core objects in Salesforce Sales Cloud for managing relationships with individuals at customer organizations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce record identifier\",\n      \"pattern\": \"^[a-zA-Z0-9]{18}$\",\n      \"readOnly\": true\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the record has been moved to the Recycle Bin\",\n      \"readOnly\": true\n    },\n    \"MasterRecordId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"If deleted as result of a merge, ID of the master record\"\
  ,\n      \"readOnly\": true\n    },\n    \"AccountId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the account that is the parent of this contact\"\n    },\n    \"LastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the contact\",\n      \"maxLength\": 80\n    },\n    \"FirstName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"First name of the contact\",\n      \"maxLength\": 40\n    },\n    \"Salutation\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Honorific abbreviation or title of the contact\",\n      \"enum\": [null, \"Mr.\", \"Ms.\", \"Mrs.\", \"Dr.\", \"Prof.\"]\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Concatenation of FirstName, MiddleName, LastName, and Suffix\",\n      \"readOnly\": true\n    },\n    \"MiddleName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Middle name of the contact\",\n      \"maxLength\"\
  : 40\n    },\n    \"Suffix\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name suffix of the contact\",\n      \"maxLength\": 40\n    },\n    \"OtherStreet\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Street address for the other address\"\n    },\n    \"OtherCity\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"City for the other address\",\n      \"maxLength\": 40\n    },\n    \"OtherState\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"State for the other address\",\n      \"maxLength\": 80\n    },\n    \"OtherPostalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Postal code for the other address\",\n      \"maxLength\": 20\n    },\n    \"OtherCountry\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Country for the other address\",\n      \"maxLength\": 80\n    },\n    \"OtherLatitude\": {\n      \"type\": [\"number\", \"null\"],\n  \
  \    \"description\": \"Latitude for the other address\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"OtherLongitude\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Longitude for the other address\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    },\n    \"MailingStreet\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Street address for the mailing address\"\n    },\n    \"MailingCity\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"City for the mailing address\",\n      \"maxLength\": 40\n    },\n    \"MailingState\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"State for the mailing address\",\n      \"maxLength\": 80\n    },\n    \"MailingPostalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Postal code for the mailing address\",\n      \"maxLength\": 20\n    },\n    \"MailingCountry\": {\n      \"type\": [\"string\", \"null\"],\n    \
  \  \"description\": \"Country for the mailing address\",\n      \"maxLength\": 80\n    },\n    \"MailingLatitude\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Latitude for the mailing address\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"MailingLongitude\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Longitude for the mailing address\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    },\n    \"Phone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Phone number for the contact\",\n      \"maxLength\": 40\n    },\n    \"Fax\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Fax number for the contact\",\n      \"maxLength\": 40\n    },\n    \"MobilePhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contact's mobile phone number\",\n      \"maxLength\": 40\n    },\n    \"HomePhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\"\
  : \"Home phone number for the contact\",\n      \"maxLength\": 40\n    },\n    \"OtherPhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Other phone number for the contact\",\n      \"maxLength\": 40\n    },\n    \"AssistantPhone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Phone number for the contact's assistant\",\n      \"maxLength\": 40\n    },\n    \"ReportsToId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the contact that this contact reports to\"\n    },\n    \"Email\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Email address for the contact\",\n      \"format\": \"email\",\n      \"maxLength\": 80\n    },\n    \"Title\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Title of the contact, such as CEO or Vice President\",\n      \"maxLength\": 128\n    },\n    \"Department\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"\
  Department of the contact\",\n      \"maxLength\": 80\n    },\n    \"AssistantName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name of the assistant\",\n      \"maxLength\": 40\n    },\n    \"LeadSource\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Source from which the contact was obtained\",\n      \"enum\": [null, \"Web\", \"Phone Inquiry\", \"Partner Referral\", \"Purchased List\", \"Other\"]\n    },\n    \"Birthdate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Birthdate for the contact\"\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Text description of the contact\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the owner of the account associated with this contact\"\n    },\n    \"HasOptedOutOfEmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the\
  \ contact has opted out of email (true) or not (false)\",\n      \"default\": false\n    },\n    \"HasOptedOutOfFax\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the contact has opted out of fax (true) or not (false)\",\n      \"default\": false\n    },\n    \"DoNotCall\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates that the contact does not want to be called\",\n      \"default\": false\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was created\",\n      \"readOnly\": true\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created this record\",\n      \"readOnly\": true\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was last modified\",\n      \"readOnly\": true\n\
  \    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified this record\",\n      \"readOnly\": true\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was last modified by a user or process\",\n      \"readOnly\": true\n    },\n    \"LastActivityDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Most recent activity date\",\n      \"readOnly\": true\n    },\n    \"LastCURequestDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Last date the contact was requested via a customer update\",\n      \"readOnly\": true\n    },\n    \"LastCUUpdateDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Last date the contact was updated via a customer update\",\n\
  \      \"readOnly\": true\n    },\n    \"EmailBouncedReason\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"If bounced, the reason for the bounce\",\n      \"maxLength\": 255\n    },\n    \"EmailBouncedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"If bounced, the date and time the bounce occurred\"\n    },\n    \"Jigsaw\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"References the ID of a contact in Data.com\",\n      \"maxLength\": 20\n    },\n    \"JigsawContactId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"References a contact in Data.com\",\n      \"readOnly\": true\n    },\n    \"CleanStatus\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Indicates the record's clean status as compared with Data.com\",\n      \"enum\": [null, \"Matched\", \"Different\", \"Acknowledged\", \"NotFound\", \"Inactive\", \"Pending\", \"SelectMatch\"\
  , \"Skipped\"]\n    },\n    \"IndividualId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the related individual record for data privacy\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Contact\"\n        },\n        \"url\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"LastName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/json-schema/salesforce-sales-cloud-contact-schema.json
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
title: Salesforce Contact
---
