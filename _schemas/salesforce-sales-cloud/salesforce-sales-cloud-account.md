---
description: Represents an individual account, which is an organization or person involved with your business (such as customers, competitors, and partners). Accounts are one of the core objects in Salesforce Sales Cloud.
layout: schema
name: Salesforce Account
properties_list:
- description: Unique 18-character Salesforce record identifier
  name: Id
  type: string
- description: Indicates whether the record has been moved to the Recycle Bin (true) or not (false)
  name: IsDeleted
  type: boolean
- description: If this record was deleted as the result of a merge, this field contains the ID of the master record
  name: MasterRecordId
  type:
  - string
  - 'null'
- description: Name of the account. Maximum 255 characters.
  name: Name
  type: string
- description: Type of account, for example, Customer, Competitor, or Partner
  name: Type
  type:
  - string
  - 'null'
- description: ID of the parent object, if any
  name: ParentId
  type:
  - string
  - 'null'
- description: Street address for the billing address of this account
  name: BillingStreet
  type:
  - string
  - 'null'
- description: City for the billing address of this account
  name: BillingCity
  type:
  - string
  - 'null'
- description: State or province for the billing address of this account
  name: BillingState
  type:
  - string
  - 'null'
- description: Postal code for the billing address of this account
  name: BillingPostalCode
  type:
  - string
  - 'null'
- description: Country for the billing address of this account
  name: BillingCountry
  type:
  - string
  - 'null'
- description: Latitude of the billing address
  name: BillingLatitude
  type:
  - number
  - 'null'
- description: Longitude of the billing address
  name: BillingLongitude
  type:
  - number
  - 'null'
- description: Street address for the shipping address of this account
  name: ShippingStreet
  type:
  - string
  - 'null'
- description: City for the shipping address of this account
  name: ShippingCity
  type:
  - string
  - 'null'
- description: State or province for the shipping address of this account
  name: ShippingState
  type:
  - string
  - 'null'
- description: Postal code for the shipping address of this account
  name: ShippingPostalCode
  type:
  - string
  - 'null'
- description: Country for the shipping address of this account
  name: ShippingCountry
  type:
  - string
  - 'null'
- description: Latitude of the shipping address
  name: ShippingLatitude
  type:
  - number
  - 'null'
- description: Longitude of the shipping address
  name: ShippingLongitude
  type:
  - number
  - 'null'
- description: Phone number for this account
  name: Phone
  type:
  - string
  - 'null'
- description: Fax number for this account
  name: Fax
  type:
  - string
  - 'null'
- description: Account number assigned to this account (external)
  name: AccountNumber
  type:
  - string
  - 'null'
- description: The website of this account
  name: Website
  type:
  - string
  - 'null'
- description: Standard Industrial Classification code of the company's main business categorization
  name: Sic
  type:
  - string
  - 'null'
- description: An industry associated with this account
  name: Industry
  type:
  - string
  - 'null'
- description: Estimated annual revenue of the account
  name: AnnualRevenue
  type:
  - number
  - 'null'
- description: Number of employees working at the company
  name: NumberOfEmployees
  type:
  - integer
  - 'null'
- description: Ownership type for the account
  name: Ownership
  type:
  - string
  - 'null'
- description: The stock ticker symbol for this account
  name: TickerSymbol
  type:
  - string
  - 'null'
- description: Text description of the account
  name: Description
  type:
  - string
  - 'null'
- description: The account's prospect rating
  name: Rating
  type:
  - string
  - 'null'
- description: Name of the account's location
  name: Site
  type:
  - string
  - 'null'
- description: ID of the user who currently owns this account
  name: OwnerId
  type: string
- description: Date and time when this record was created
  name: CreatedDate
  type: string
- description: ID of the user who created this record
  name: CreatedById
  type: string
- description: Date and time when a user last modified this record
  name: LastModifiedDate
  type: string
- description: ID of the user who last updated this record
  name: LastModifiedById
  type: string
- description: Date and time when this record was last modified by a user or automated process
  name: SystemModstamp
  type: string
- description: Value is the most recent of either the due date of the most recent event or the due date of the most recently closed task
  name: LastActivityDate
  type:
  - string
  - 'null'
- description: References the ID of a company in Data.com
  name: Jigsaw
  type:
  - string
  - 'null'
- description: References a company in Data.com
  name: JigsawCompanyId
  type:
  - string
  - 'null'
- description: Indicates the record's clean status as compared with Data.com
  name: CleanStatus
  type:
  - string
  - 'null'
- description: The source of the account record
  name: AccountSource
  type:
  - string
  - 'null'
- description: The Dun & Bradstreet Data Universal Numbering System (D-U-N-S) number
  name: DunsNumber
  type:
  - string
  - 'null'
- description: A name, different from its legal name, that an org may use for conducting business
  name: Tradestyle
  type:
  - string
  - 'null'
- description: The six-digit North American Industry Classification System (NAICS) code
  name: NaicsCode
  type:
  - string
  - 'null'
- description: A brief description of an organization's line of business
  name: NaicsDesc
  type:
  - string
  - 'null'
- description: The year the organization was legally established
  name: YearStarted
  type:
  - string
  - 'null'
- description: A brief description of the organization's line of business based on SIC code
  name: SicDesc
  type:
  - string
  - 'null'
- description: The operating hours associated with the account
  name: OperatingHoursId
  type:
  - string
  - 'null'
- description: sObject metadata attributes
  name: attributes
  type: object
provider_name: Salesforce Sales Cloud
provider_slug: salesforce-sales-cloud
schema_file: json-schema/salesforce-sales-cloud-account-schema.json
slug: salesforce-sales-cloud-account
source_filename: salesforce-sales-cloud-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/sales-cloud/account.json\",\n  \"title\": \"Salesforce Account\",\n  \"description\": \"Represents an individual account, which is an organization or person involved with your business (such as customers, competitors, and partners). Accounts are one of the core objects in Salesforce Sales Cloud.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce record identifier\",\n      \"pattern\": \"^[a-zA-Z0-9]{18}$\",\n      \"readOnly\": true\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the record has been moved to the Recycle Bin (true) or not (false)\",\n      \"readOnly\": true\n    },\n    \"MasterRecordId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"If this record was deleted\
  \ as the result of a merge, this field contains the ID of the master record\",\n      \"readOnly\": true\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the account. Maximum 255 characters.\",\n      \"maxLength\": 255\n    },\n    \"Type\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Type of account, for example, Customer, Competitor, or Partner\",\n      \"enum\": [\n        null,\n        \"Prospect\",\n        \"Customer - Direct\",\n        \"Customer - Channel\",\n        \"Channel Partner / Reseller\",\n        \"Installation Partner\",\n        \"Technology Partner\",\n        \"Other\"\n      ]\n    },\n    \"ParentId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the parent object, if any\"\n    },\n    \"BillingStreet\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Street address for the billing address of this account\"\n    },\n    \"BillingCity\": {\n  \
  \    \"type\": [\"string\", \"null\"],\n      \"description\": \"City for the billing address of this account\",\n      \"maxLength\": 40\n    },\n    \"BillingState\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"State or province for the billing address of this account\",\n      \"maxLength\": 80\n    },\n    \"BillingPostalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Postal code for the billing address of this account\",\n      \"maxLength\": 20\n    },\n    \"BillingCountry\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Country for the billing address of this account\",\n      \"maxLength\": 80\n    },\n    \"BillingLatitude\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Latitude of the billing address\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"BillingLongitude\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Longitude of the billing\
  \ address\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    },\n    \"ShippingStreet\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Street address for the shipping address of this account\"\n    },\n    \"ShippingCity\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"City for the shipping address of this account\",\n      \"maxLength\": 40\n    },\n    \"ShippingState\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"State or province for the shipping address of this account\",\n      \"maxLength\": 80\n    },\n    \"ShippingPostalCode\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Postal code for the shipping address of this account\",\n      \"maxLength\": 20\n    },\n    \"ShippingCountry\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Country for the shipping address of this account\",\n      \"maxLength\": 80\n    },\n    \"ShippingLatitude\": {\n      \"type\"\
  : [\"number\", \"null\"],\n      \"description\": \"Latitude of the shipping address\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"ShippingLongitude\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Longitude of the shipping address\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    },\n    \"Phone\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Phone number for this account\",\n      \"maxLength\": 40\n    },\n    \"Fax\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Fax number for this account\",\n      \"maxLength\": 40\n    },\n    \"AccountNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Account number assigned to this account (external)\",\n      \"maxLength\": 40\n    },\n    \"Website\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The website of this account\",\n      \"format\": \"uri\",\n      \"maxLength\": 255\n    },\n    \"\
  Sic\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Standard Industrial Classification code of the company's main business categorization\",\n      \"maxLength\": 20\n    },\n    \"Industry\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"An industry associated with this account\",\n      \"enum\": [\n        null,\n        \"Agriculture\",\n        \"Apparel\",\n        \"Banking\",\n        \"Biotechnology\",\n        \"Chemicals\",\n        \"Communications\",\n        \"Construction\",\n        \"Consulting\",\n        \"Education\",\n        \"Electronics\",\n        \"Energy\",\n        \"Engineering\",\n        \"Entertainment\",\n        \"Environmental\",\n        \"Finance\",\n        \"Food & Beverage\",\n        \"Government\",\n        \"Healthcare\",\n        \"Hospitality\",\n        \"Insurance\",\n        \"Machinery\",\n        \"Manufacturing\",\n        \"Media\",\n        \"Not For Profit\",\n        \"Recreation\",\n\
  \        \"Retail\",\n        \"Shipping\",\n        \"Technology\",\n        \"Telecommunications\",\n        \"Transportation\",\n        \"Utilities\",\n        \"Other\"\n      ]\n    },\n    \"AnnualRevenue\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Estimated annual revenue of the account\"\n    },\n    \"NumberOfEmployees\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Number of employees working at the company\"\n    },\n    \"Ownership\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Ownership type for the account\",\n      \"enum\": [null, \"Public\", \"Private\", \"Subsidiary\", \"Other\"]\n    },\n    \"TickerSymbol\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The stock ticker symbol for this account\",\n      \"maxLength\": 20\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Text description of the account\"\n    },\n    \"\
  Rating\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The account's prospect rating\",\n      \"enum\": [null, \"Hot\", \"Warm\", \"Cold\"]\n    },\n    \"Site\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name of the account's location\",\n      \"maxLength\": 80\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who currently owns this account\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was created\",\n      \"readOnly\": true\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created this record\",\n      \"readOnly\": true\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when a user last modified this record\",\n      \"readOnly\": true\n\
  \    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last updated this record\",\n      \"readOnly\": true\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was last modified by a user or automated process\",\n      \"readOnly\": true\n    },\n    \"LastActivityDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Value is the most recent of either the due date of the most recent event or the due date of the most recently closed task\",\n      \"readOnly\": true\n    },\n    \"Jigsaw\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"References the ID of a company in Data.com\",\n      \"maxLength\": 20\n    },\n    \"JigsawCompanyId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"References a company in Data.com\",\n      \"readOnly\"\
  : true\n    },\n    \"CleanStatus\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Indicates the record's clean status as compared with Data.com\",\n      \"enum\": [null, \"Matched\", \"Different\", \"Acknowledged\", \"NotFound\", \"Inactive\", \"Pending\", \"SelectMatch\", \"Skipped\"]\n    },\n    \"AccountSource\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The source of the account record\",\n      \"enum\": [null, \"Web\", \"Phone Inquiry\", \"Partner Referral\", \"Purchased List\", \"Other\"]\n    },\n    \"DunsNumber\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The Dun & Bradstreet Data Universal Numbering System (D-U-N-S) number\",\n      \"maxLength\": 9\n    },\n    \"Tradestyle\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A name, different from its legal name, that an org may use for conducting business\",\n      \"maxLength\": 255\n    },\n    \"NaicsCode\": {\n      \"type\"\
  : [\"string\", \"null\"],\n      \"description\": \"The six-digit North American Industry Classification System (NAICS) code\",\n      \"maxLength\": 8\n    },\n    \"NaicsDesc\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A brief description of an organization's line of business\",\n      \"maxLength\": 120\n    },\n    \"YearStarted\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The year the organization was legally established\",\n      \"maxLength\": 4\n    },\n    \"SicDesc\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A brief description of the organization's line of business based on SIC code\",\n      \"maxLength\": 80\n    },\n    \"OperatingHoursId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The operating hours associated with the account\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"sObject metadata attributes\",\n      \"properties\"\
  : {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Account\"\n        },\n        \"url\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"Name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/json-schema/salesforce-sales-cloud-account-schema.json
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
title: Salesforce Account
---
