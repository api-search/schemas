---
description: Represents a marketing campaign, such as a direct mail promotion, webinar, or trade show. Campaigns organize marketing efforts and track their effectiveness by associating leads, contacts, and opportunities.
layout: schema
name: Salesforce Campaign
properties_list:
- description: Unique 18-character Salesforce record identifier
  name: Id
  type: string
- description: Indicates whether the record has been moved to the Recycle Bin
  name: IsDeleted
  type: boolean
- description: Name of the campaign
  name: Name
  type: string
- description: ID of the parent campaign for campaign hierarchy
  name: ParentId
  type:
  - string
  - 'null'
- description: Type of campaign
  name: Type
  type:
  - string
  - 'null'
- description: Status of the campaign
  name: Status
  type:
  - string
  - 'null'
- description: Starting date for the campaign
  name: StartDate
  type:
  - string
  - 'null'
- description: Ending date for the campaign
  name: EndDate
  type:
  - string
  - 'null'
- description: Amount of revenue expected from the campaign
  name: ExpectedRevenue
  type:
  - number
  - 'null'
- description: Amount budgeted for the campaign
  name: BudgetedCost
  type:
  - number
  - 'null'
- description: Actual amount spent on the campaign
  name: ActualCost
  type:
  - number
  - 'null'
- description: Percentage of expected response for the campaign
  name: ExpectedResponse
  type:
  - number
  - 'null'
- description: Number of individuals targeted by the campaign
  name: NumberSent
  type:
  - number
  - 'null'
- description: Indicates whether the campaign is active
  name: IsActive
  type: boolean
- description: Text description of the campaign
  name: Description
  type:
  - string
  - 'null'
- description: Number of leads associated with the campaign
  name: NumberOfLeads
  type: integer
- description: Number of leads converted to contacts from the campaign
  name: NumberOfConvertedLeads
  type: integer
- description: Number of contacts associated with the campaign
  name: NumberOfContacts
  type: integer
- description: Number of campaign members that have responded
  name: NumberOfResponses
  type: integer
- description: Number of won opportunities associated with the campaign
  name: NumberOfWonOpportunities
  type: integer
- description: Number of opportunities associated with the campaign
  name: NumberOfOpportunities
  type: integer
- description: Total amount of all opportunities associated with the campaign
  name: AmountAllOpportunities
  type:
  - number
  - 'null'
- description: Total amount of won opportunities
  name: AmountWonOpportunities
  type:
  - number
  - 'null'
- description: ID of the user who owns the campaign
  name: OwnerId
  type: string
- description: ''
  name: CreatedDate
  type: string
- description: ''
  name: CreatedById
  type: string
- description: ''
  name: LastModifiedDate
  type: string
- description: ''
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
- description: The record type for campaign members
  name: CampaignMemberRecordTypeId
  type:
  - string
  - 'null'
- description: ''
  name: attributes
  type: object
provider_name: Salesforce Sales Cloud
provider_slug: salesforce-sales-cloud
schema_file: json-schema/salesforce-sales-cloud-campaign-schema.json
slug: salesforce-sales-cloud-campaign
source_filename: salesforce-sales-cloud-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/sales-cloud/campaign.json\",\n  \"title\": \"Salesforce Campaign\",\n  \"description\": \"Represents a marketing campaign, such as a direct mail promotion, webinar, or trade show. Campaigns organize marketing efforts and track their effectiveness by associating leads, contacts, and opportunities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce record identifier\",\n      \"pattern\": \"^[a-zA-Z0-9]{18}$\",\n      \"readOnly\": true\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the record has been moved to the Recycle Bin\",\n      \"readOnly\": true\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the campaign\",\n      \"maxLength\": 80\n    },\n    \"ParentId\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the parent campaign for campaign hierarchy\"\n    },\n    \"Type\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Type of campaign\",\n      \"enum\": [null, \"Conference\", \"Webinar\", \"Trade Show\", \"Public Relations\", \"Partners\", \"Referral Program\", \"Advertisement\", \"Banner Ads\", \"Direct Mail\", \"Email\", \"Telemarketing\", \"Other\"]\n    },\n    \"Status\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Status of the campaign\",\n      \"enum\": [null, \"Planned\", \"In Progress\", \"Completed\", \"Aborted\"]\n    },\n    \"StartDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Starting date for the campaign\"\n    },\n    \"EndDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Ending date for the campaign\"\n    },\n    \"ExpectedRevenue\"\
  : {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Amount of revenue expected from the campaign\"\n    },\n    \"BudgetedCost\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Amount budgeted for the campaign\"\n    },\n    \"ActualCost\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Actual amount spent on the campaign\"\n    },\n    \"ExpectedResponse\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Percentage of expected response for the campaign\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"NumberSent\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Number of individuals targeted by the campaign\"\n    },\n    \"IsActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the campaign is active\",\n      \"default\": false\n    },\n    \"Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Text description\
  \ of the campaign\"\n    },\n    \"NumberOfLeads\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of leads associated with the campaign\",\n      \"readOnly\": true\n    },\n    \"NumberOfConvertedLeads\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of leads converted to contacts from the campaign\",\n      \"readOnly\": true\n    },\n    \"NumberOfContacts\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of contacts associated with the campaign\",\n      \"readOnly\": true\n    },\n    \"NumberOfResponses\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of campaign members that have responded\",\n      \"readOnly\": true\n    },\n    \"NumberOfWonOpportunities\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of won opportunities associated with the campaign\",\n      \"readOnly\": true\n    },\n    \"NumberOfOpportunities\": {\n      \"type\": \"integer\",\n      \"description\": \"Number\
  \ of opportunities associated with the campaign\",\n      \"readOnly\": true\n    },\n    \"AmountAllOpportunities\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Total amount of all opportunities associated with the campaign\",\n      \"readOnly\": true\n    },\n    \"AmountWonOpportunities\": {\n      \"type\": [\"number\", \"null\"],\n      \"description\": \"Total amount of won opportunities\",\n      \"readOnly\": true\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who owns the campaign\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n\
  \    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"LastActivityDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"readOnly\": true\n    },\n    \"CampaignMemberRecordTypeId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The record type for campaign members\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Campaign\"\n        },\n        \"url\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"Name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/json-schema/salesforce-sales-cloud-campaign-schema.json
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
title: Salesforce Campaign
---
