---
description: Represents an opportunity, which is a sale or pending deal. Opportunities are one of the core objects in Salesforce Sales Cloud for tracking the sales pipeline, revenue forecasting, and deal management.
layout: schema
name: Salesforce Opportunity
properties_list:
- description: Unique 18-character Salesforce record identifier
  name: Id
  type: string
- description: Indicates whether the record has been moved to the Recycle Bin
  name: IsDeleted
  type: boolean
- description: ID of the account associated with this opportunity
  name: AccountId
  type:
  - string
  - 'null'
- description: A name for this opportunity
  name: Name
  type: string
- description: Text description of the opportunity
  name: Description
  type:
  - string
  - 'null'
- description: Current stage of this opportunity in the sales process
  name: StageName
  type: string
- description: Estimated total sale amount
  name: Amount
  type:
  - number
  - 'null'
- description: Percentage of estimated confidence in closing the opportunity
  name: Probability
  type:
  - number
  - 'null'
- description: Calculated revenue based on the Amount field multiplied by the Probability
  name: ExpectedRevenue
  type:
  - number
  - 'null'
- description: Number of items included in this opportunity
  name: TotalOpportunityQuantity
  type:
  - number
  - 'null'
- description: Date when the opportunity is expected to close
  name: CloseDate
  type: string
- description: Type of opportunity
  name: Type
  type:
  - string
  - 'null'
- description: Description of the next step in the sales process
  name: NextStep
  type:
  - string
  - 'null'
- description: Source of this opportunity
  name: LeadSource
  type:
  - string
  - 'null'
- description: Indicates whether the opportunity is closed
  name: IsClosed
  type: boolean
- description: Indicates whether the opportunity is won
  name: IsWon
  type: boolean
- description: Forecast category determined by the Stage
  name: ForecastCategory
  type:
  - string
  - 'null'
- description: Name of the forecast category
  name: ForecastCategoryName
  type:
  - string
  - 'null'
- description: ID of the campaign that generated this opportunity
  name: CampaignId
  type:
  - string
  - 'null'
- description: Indicates whether the opportunity has associated opportunity products
  name: HasOpportunityLineItem
  type: boolean
- description: ID of the price book associated with this opportunity
  name: Pricebook2Id
  type:
  - string
  - 'null'
- description: ID of the user who owns this opportunity
  name: OwnerId
  type: string
- description: ID of the primary contact for this opportunity
  name: ContactId
  type:
  - string
  - 'null'
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
- description: The fiscal quarter for the close date
  name: FiscalQuarter
  type:
  - integer
  - 'null'
- description: The fiscal year for the close date
  name: FiscalYear
  type:
  - integer
  - 'null'
- description: The fiscal period for the close date
  name: Fiscal
  type:
  - string
  - 'null'
- description: Date when the opportunity stage was last changed
  name: LastStageChangeDate
  type:
  - string
  - 'null'
- description: Indicates whether there is an open activity for the opportunity
  name: HasOpenActivity
  type: boolean
- description: Indicates whether there is an overdue task for the opportunity
  name: HasOverdueTask
  type: boolean
- description: ''
  name: LastAmountChangedHistoryId
  type:
  - string
  - 'null'
- description: ''
  name: LastCloseDateChangedHistoryId
  type:
  - string
  - 'null'
- description: ''
  name: attributes
  type: object
provider_name: Salesforce Sales Cloud
provider_slug: salesforce-sales-cloud
schema_file: json-schema/salesforce-sales-cloud-opportunity-schema.json
slug: salesforce-sales-cloud-opportunity
source_filename: salesforce-sales-cloud-opportunity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/sales-cloud/opportunity.json\",\n  \"title\": \"Salesforce Opportunity\",\n  \"description\": \"Represents an opportunity, which is a sale or pending deal. Opportunities are one of the core objects in Salesforce Sales Cloud for tracking the sales pipeline, revenue forecasting, and deal management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce record identifier\",\n      \"pattern\": \"^[a-zA-Z0-9]{18}$\",\n      \"readOnly\": true\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the record has been moved to the Recycle Bin\",\n      \"readOnly\": true\n    },\n    \"AccountId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the account associated with this opportunity\"\
  \n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"A name for this opportunity\",\n      \"maxLength\": 120\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Text description of the opportunity\"\n    },\n    \"StageName\": {\n      \"type\": \"string\",\n      \"description\": \"Current stage of this opportunity in the sales process\",\n      \"enum\": [\n        \"Prospecting\",\n        \"Qualification\",\n        \"Needs Analysis\",\n        \"Value Proposition\",\n        \"Id. Decision Makers\",\n        \"Perception Analysis\",\n        \"Proposal/Price Quote\",\n        \"Negotiation/Review\",\n        \"Closed Won\",\n        \"Closed Lost\"\n      ]\n    },\n    \"Amount\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Estimated total sale amount\"\n    },\n    \"Probability\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Percentage of estimated confidence\
  \ in closing the opportunity\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"ExpectedRevenue\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Calculated revenue based on the Amount field multiplied by the Probability\",\n      \"readOnly\": true\n    },\n    \"TotalOpportunityQuantity\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Number of items included in this opportunity\"\n    },\n    \"CloseDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the opportunity is expected to close\"\n    },\n    \"Type\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Type of opportunity\",\n      \"enum\": [null, \"Existing Customer - Upgrade\", \"Existing Customer - Replacement\", \"Existing Customer - Downgrade\", \"New Customer\"]\n    },\n    \"NextStep\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Description of the next step in the\
  \ sales process\",\n      \"maxLength\": 255\n    },\n    \"LeadSource\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Source of this opportunity\",\n      \"enum\": [null, \"Web\", \"Phone Inquiry\", \"Partner Referral\", \"Purchased List\", \"Other\"]\n    },\n    \"IsClosed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the opportunity is closed\",\n      \"readOnly\": true\n    },\n    \"IsWon\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the opportunity is won\",\n      \"readOnly\": true\n    },\n    \"ForecastCategory\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Forecast category determined by the Stage\",\n      \"enum\": [null, \"Omitted\", \"Pipeline\", \"BestCase\", \"MostLikely\", \"Forecast\", \"Closed\"],\n      \"readOnly\": true\n    },\n    \"ForecastCategoryName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name of the forecast\
  \ category\",\n      \"enum\": [null, \"Omitted\", \"Pipeline\", \"Best Case\", \"Most Likely\", \"Commit\", \"Closed\"]\n    },\n    \"CampaignId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the campaign that generated this opportunity\"\n    },\n    \"HasOpportunityLineItem\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the opportunity has associated opportunity products\",\n      \"readOnly\": true\n    },\n    \"Pricebook2Id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the price book associated with this opportunity\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who owns this opportunity\"\n    },\n    \"ContactId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the primary contact for this opportunity\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n     \
  \ \"description\": \"Date and time when this record was created\",\n      \"readOnly\": true\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created this record\",\n      \"readOnly\": true\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was last modified\",\n      \"readOnly\": true\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified this record\",\n      \"readOnly\": true\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"LastActivityDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"readOnly\": true\n    },\n    \"FiscalQuarter\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The fiscal quarter for\
  \ the close date\",\n      \"readOnly\": true\n    },\n    \"FiscalYear\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The fiscal year for the close date\",\n      \"readOnly\": true\n    },\n    \"Fiscal\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The fiscal period for the close date\",\n      \"readOnly\": true\n    },\n    \"LastStageChangeDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date when the opportunity stage was last changed\",\n      \"readOnly\": true\n    },\n    \"HasOpenActivity\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether there is an open activity for the opportunity\",\n      \"readOnly\": true\n    },\n    \"HasOverdueTask\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether there is an overdue task for the opportunity\",\n      \"readOnly\": true\n    },\n    \"LastAmountChangedHistoryId\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"readOnly\": true\n    },\n    \"LastCloseDateChangedHistoryId\": {\n      \"type\": [\"string\", \"null\"],\n      \"readOnly\": true\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Opportunity\"\n        },\n        \"url\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"Name\", \"StageName\", \"CloseDate\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/json-schema/salesforce-sales-cloud-opportunity-schema.json
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
title: Salesforce Opportunity
---
