---
description: ''
layout: schema
name: Record14
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: Id
  type: string
- description: ''
  name: IsDeleted
  type: boolean
- description: ''
  name: MasterRecordId
  type: '[''string'', ''null'']'
- description: ''
  name: Name
  type: string
- description: ''
  name: Type
  type: string
- description: ''
  name: ParentId
  type: '[''string'', ''null'']'
- description: ''
  name: BillingStreet
  type: string
- description: ''
  name: BillingCity
  type: string
- description: ''
  name: BillingState
  type: string
- description: ''
  name: BillingPostalCode
  type: '[''string'', ''null'']'
- description: ''
  name: BillingCountry
  type: '[''string'', ''null'']'
- description: ''
  name: BillingLatitude
  type: '[''string'', ''null'']'
- description: ''
  name: BillingLongitude
  type: '[''string'', ''null'']'
- description: ''
  name: BillingGeocodeAccuracy
  type: '[''string'', ''null'']'
- description: ''
  name: BillingAddress
  type: object
- description: ''
  name: ShippingStreet
  type: '[''string'', ''null'']'
- description: ''
  name: ShippingCity
  type: '[''string'', ''null'']'
- description: ''
  name: ShippingState
  type: '[''string'', ''null'']'
- description: ''
  name: ShippingPostalCode
  type: '[''string'', ''null'']'
- description: ''
  name: ShippingCountry
  type: '[''string'', ''null'']'
- description: ''
  name: ShippingLatitude
  type: '[''string'', ''null'']'
- description: ''
  name: ShippingLongitude
  type: '[''string'', ''null'']'
- description: ''
  name: ShippingGeocodeAccuracy
  type: '[''string'', ''null'']'
- description: ''
  name: ShippingAddress
  type: object
- description: ''
  name: Phone
  type: string
- description: ''
  name: Fax
  type: string
- description: ''
  name: AccountNumber
  type: string
- description: ''
  name: Website
  type: string
- description: ''
  name: PhotoUrl
  type: string
- description: ''
  name: Sic
  type: string
- description: ''
  name: Industry
  type: string
- description: ''
  name: AnnualRevenue
  type: integer
- description: ''
  name: NumberOfEmployees
  type: integer
- description: ''
  name: Ownership
  type: string
- description: ''
  name: TickerSymbol
  type: '[''string'', ''null'']'
- description: ''
  name: Description
  type: '[''string'', ''null'']'
- description: ''
  name: Rating
  type: '[''string'', ''null'']'
- description: ''
  name: Site
  type: '[''string'', ''null'']'
- description: ''
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
  type: '[''string'', ''null'']'
- description: ''
  name: LastViewedDate
  type: '[''string'', ''null'']'
- description: ''
  name: LastReferencedDate
  type: '[''string'', ''null'']'
- description: ''
  name: IsPartner
  type: boolean
- description: ''
  name: IsCustomerPortal
  type: boolean
- description: ''
  name: ChannelProgramName
  type: '[''string'', ''null'']'
- description: ''
  name: ChannelProgramLevelName
  type: '[''string'', ''null'']'
- description: ''
  name: Jigsaw
  type: '[''string'', ''null'']'
- description: ''
  name: JigsawCompanyId
  type: '[''string'', ''null'']'
- description: ''
  name: CleanStatus
  type: string
- description: ''
  name: AccountSource
  type: '[''string'', ''null'']'
- description: ''
  name: DunsNumber
  type: '[''string'', ''null'']'
- description: ''
  name: Tradestyle
  type: '[''string'', ''null'']'
- description: ''
  name: NaicsCode
  type: '[''string'', ''null'']'
- description: ''
  name: NaicsDesc
  type: '[''string'', ''null'']'
- description: ''
  name: YearStarted
  type: '[''string'', ''null'']'
- description: ''
  name: SicDesc
  type: '[''string'', ''null'']'
- description: ''
  name: DandbCompanyId
  type: '[''string'', ''null'']'
- description: ''
  name: CustomerPriority__c
  type: '[''string'', ''null'']'
- description: ''
  name: SLA__c
  type: string
- description: ''
  name: Active__c
  type: '[''string'', ''null'']'
- description: ''
  name: NumberofLocations__c
  type: integer
- description: ''
  name: UpsellOpportunity__c
  type: string
- description: ''
  name: SLASerialNumber__c
  type: string
- description: ''
  name: SLAExpirationDate__c
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record14-schema.json
slug: salesforce-record14
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"url\"\n      ]\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"MasterRecordId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"ParentId\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n\
  \    },\n    \"BillingStreet\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"BillingCity\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"BillingState\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"BillingPostalCode\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"BillingCountry\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": 42\n    },\n    \"BillingLatitude\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"BillingLongitude\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"BillingGeocodeAccuracy\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"BillingAddress\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"city\": {\n          \"type\":\
  \ \"string\",\n          \"example\": \"example_value\"\n        },\n        \"country\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": 42\n        },\n        \"geocodeAccuracy\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"latitude\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"longitude\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"postalCode\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"street\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"city\",\n        \"country\",\n        \"geocodeAccuracy\"\
  ,\n        \"latitude\",\n        \"longitude\",\n        \"postalCode\",\n        \"state\",\n        \"street\"\n      ]\n    },\n    \"ShippingStreet\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"ShippingCity\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"ShippingState\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"ShippingPostalCode\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"ShippingCountry\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": 42\n    },\n    \"ShippingLatitude\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"ShippingLongitude\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"ShippingGeocodeAccuracy\": {\n      \"type\": \"['string', 'null']\",\n\
  \      \"example\": \"example_value\"\n    },\n    \"ShippingAddress\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"Phone\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Fax\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"AccountNumber\": {\n      \"type\": \"string\",\n      \"example\": 42\n    },\n    \"Website\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"PhotoUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"Sic\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Industry\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"AnnualRevenue\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"NumberOfEmployees\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"Ownership\"\
  : {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"TickerSymbol\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"Description\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"A sample description.\"\n    },\n    \"Rating\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"Site\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n\
  \    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"LastActivityDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"LastViewedDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"LastReferencedDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"IsPartner\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"IsCustomerPortal\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"ChannelProgramName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"ChannelProgramLevelName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"Jigsaw\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"JigsawCompanyId\":\
  \ {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"500123\"\n    },\n    \"CleanStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"AccountSource\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": 42\n    },\n    \"DunsNumber\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"Tradestyle\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"NaicsCode\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"NaicsDesc\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"YearStarted\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"SicDesc\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"DandbCompanyId\": {\n      \"type\": \"['string', 'null']\"\
  ,\n      \"example\": \"500123\"\n    },\n    \"CustomerPriority__c\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"SLA__c\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Active__c\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"NumberofLocations__c\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"UpsellOpportunity__c\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"SLASerialNumber__c\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"SLAExpirationDate__c\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"attributes\",\n    \"Id\",\n    \"IsDeleted\",\n    \"MasterRecordId\",\n    \"Name\",\n    \"Type\",\n    \"ParentId\",\n    \"BillingStreet\",\n    \"BillingCity\",\n    \"BillingState\",\n\
  \    \"BillingPostalCode\",\n    \"BillingCountry\",\n    \"BillingLatitude\",\n    \"BillingLongitude\",\n    \"BillingGeocodeAccuracy\",\n    \"BillingAddress\",\n    \"ShippingStreet\",\n    \"ShippingCity\",\n    \"ShippingState\",\n    \"ShippingPostalCode\",\n    \"ShippingCountry\",\n    \"ShippingLatitude\",\n    \"ShippingLongitude\",\n    \"ShippingGeocodeAccuracy\",\n    \"ShippingAddress\",\n    \"Phone\",\n    \"Fax\",\n    \"AccountNumber\",\n    \"Website\",\n    \"PhotoUrl\",\n    \"Sic\",\n    \"Industry\",\n    \"AnnualRevenue\",\n    \"NumberOfEmployees\",\n    \"Ownership\",\n    \"TickerSymbol\",\n    \"Description\",\n    \"Rating\",\n    \"Site\",\n    \"OwnerId\",\n    \"CreatedDate\",\n    \"CreatedById\",\n    \"LastModifiedDate\",\n    \"LastModifiedById\",\n    \"SystemModstamp\",\n    \"LastActivityDate\",\n    \"LastViewedDate\",\n    \"LastReferencedDate\",\n    \"IsPartner\",\n    \"IsCustomerPortal\",\n    \"ChannelProgramName\",\n    \"ChannelProgramLevelName\"\
  ,\n    \"Jigsaw\",\n    \"JigsawCompanyId\",\n    \"CleanStatus\",\n    \"AccountSource\",\n    \"DunsNumber\",\n    \"Tradestyle\",\n    \"NaicsCode\",\n    \"NaicsDesc\",\n    \"YearStarted\",\n    \"SicDesc\",\n    \"DandbCompanyId\",\n    \"CustomerPriority__c\",\n    \"SLA__c\",\n    \"Active__c\",\n    \"NumberofLocations__c\",\n    \"UpsellOpportunity__c\",\n    \"SLASerialNumber__c\",\n    \"SLAExpirationDate__c\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Record14\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record14-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Record14
---
