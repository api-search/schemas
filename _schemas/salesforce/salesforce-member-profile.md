---
description: ''
layout: schema
name: MemberProfile
properties_list:
- description: ''
  name: additionalLoyaltyProgramMemberFields
  type: object
- description: ''
  name: associatedAccount
  type: '[''string'', ''null'']'
- description: ''
  name: associatedContact
  type: object
- description: ''
  name: canReceivePartnerPromotions
  type: boolean
- description: ''
  name: canReceivePromotions
  type: boolean
- description: ''
  name: enrollmentChannel
  type: string
- description: ''
  name: enrollmentDate
  type: string
- description: ''
  name: groupCreatedByMember
  type: '[''string'', ''null'']'
- description: ''
  name: groupName
  type: '[''string'', ''null'']'
- description: ''
  name: lastActivityDate
  type: '[''string'', ''null'']'
- description: ''
  name: loyaltyProgramMemberId
  type: string
- description: ''
  name: loyaltyProgramName
  type: string
- description: ''
  name: memberCurrencies
  type: array
- description: ''
  name: memberStatus
  type: string
- description: ''
  name: memberTiers
  type: array
- description: ''
  name: memberType
  type: string
- description: ''
  name: membershipEndDate
  type: string
- description: ''
  name: membershipLastRenewalDate
  type: '[''string'', ''null'']'
- description: ''
  name: membershipNumber
  type: string
- description: ''
  name: referredBy
  type: '[''string'', ''null'']'
- description: ''
  name: relatedCorporateMembershipNumber
  type: '[''string'', ''null'']'
- description: ''
  name: transactionJournalStatementFrequency
  type: string
- description: ''
  name: transactionJournalStatementLastGeneratedDate
  type: '[''string'', ''null'']'
- description: ''
  name: transactionJournalStatementMethod
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-member-profile-schema.json
slug: salesforce-member-profile
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalLoyaltyProgramMemberFields\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"associatedAccount\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": 42\n    },\n    \"associatedContact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"contactId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"example\": \"user@example.com\"\n        },\n        \"firstName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"lastName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"contactId\",\n        \"email\",\n        \"firstName\",\n        \"lastName\"\n      ]\n    },\n    \"canReceivePartnerPromotions\": {\n      \"\
  type\": \"boolean\",\n      \"example\": true\n    },\n    \"canReceivePromotions\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"enrollmentChannel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"enrollmentDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"groupCreatedByMember\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"groupName\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"lastActivityDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"loyaltyProgramMemberId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"loyaltyProgramName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"memberCurrencies\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n\
  \      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"additionalLoyaltyMemberCurrencyFields\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Level_Before_Reset__c\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"Level_Before_Reset__c\"\n            ]\n          },\n          \"escrowPointsBalance\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"expirablePoints\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"lastAccrualProcessedDate\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"lastEscrowProcessedDate\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\
  \n          },\n          \"lastExpirationProcessRunDate\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"lastPointsAggregationDate\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"lastPointsResetDate\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"loyaltyMemberCurrencyName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"loyaltyProgramCurrencyId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"loyaltyProgramCurrencyName\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"memberCurrencyId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n  \
  \        \"nextQualifyingPointsResetDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"pointsBalance\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"qualifyingPointsBalanceBeforeReset\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"totalEscrowPointsAccrued\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          },\n          \"totalEscrowRolloverPoints\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          },\n          \"totalPointsAccrued\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          },\n          \"totalPointsExpired\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          },\n          \"totalPointsRedeemed\": {\n            \"type\": \"integer\",\n            \"example\": 42\n          }\n        },\n        \"required\"\
  : [\n          \"additionalLoyaltyMemberCurrencyFields\",\n          \"escrowPointsBalance\",\n          \"expirablePoints\",\n          \"lastAccrualProcessedDate\",\n          \"lastEscrowProcessedDate\",\n          \"lastExpirationProcessRunDate\",\n          \"lastPointsAggregationDate\",\n          \"lastPointsResetDate\",\n          \"loyaltyMemberCurrencyName\",\n          \"loyaltyProgramCurrencyId\",\n          \"loyaltyProgramCurrencyName\",\n          \"memberCurrencyId\",\n          \"nextQualifyingPointsResetDate\",\n          \"pointsBalance\",\n          \"qualifyingPointsBalanceBeforeReset\",\n          \"totalEscrowPointsAccrued\",\n          \"totalEscrowRolloverPoints\",\n          \"totalPointsAccrued\",\n          \"totalPointsExpired\",\n          \"totalPointsRedeemed\"\n        ]\n      }\n    },\n    \"memberStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"memberTiers\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"additionalLoyaltyMemberTierFields\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          },\n          \"areTierBenefitsAssigned\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"loyaltyMemberTierId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"loyaltyMemberTierName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"tierChangeReason\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"tierChangeReasonType\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"tierEffectiveDate\": {\n            \"type\": \"string\",\n        \
  \    \"example\": \"example_value\"\n          },\n          \"tierExpirationDate\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"tierGroupId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"tierGroupName\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"tierId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"tierSequenceNumber\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          }\n        },\n        \"required\": [\n          \"additionalLoyaltyMemberTierFields\",\n          \"areTierBenefitsAssigned\",\n          \"loyaltyMemberTierId\",\n          \"loyaltyMemberTierName\",\n          \"tierChangeReason\",\n          \"tierChangeReasonType\",\n          \"tierEffectiveDate\",\n          \"tierExpirationDate\"\
  ,\n          \"tierGroupId\",\n          \"tierGroupName\",\n          \"tierId\",\n          \"tierSequenceNumber\"\n        ]\n      }\n    },\n    \"memberType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"membershipEndDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"membershipLastRenewalDate\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"membershipNumber\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"referredBy\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"relatedCorporateMembershipNumber\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"transactionJournalStatementFrequency\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"transactionJournalStatementLastGeneratedDate\": {\n\
  \      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"transactionJournalStatementMethod\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"additionalLoyaltyProgramMemberFields\",\n    \"associatedAccount\",\n    \"associatedContact\",\n    \"canReceivePartnerPromotions\",\n    \"canReceivePromotions\",\n    \"enrollmentChannel\",\n    \"enrollmentDate\",\n    \"groupCreatedByMember\",\n    \"groupName\",\n    \"lastActivityDate\",\n    \"loyaltyProgramMemberId\",\n    \"loyaltyProgramName\",\n    \"memberCurrencies\",\n    \"memberStatus\",\n    \"memberTiers\",\n    \"memberType\",\n    \"membershipEndDate\",\n    \"membershipLastRenewalDate\",\n    \"membershipNumber\",\n    \"referredBy\",\n    \"relatedCorporateMembershipNumber\",\n    \"transactionJournalStatementFrequency\",\n    \"transactionJournalStatementLastGeneratedDate\",\n    \"transactionJournalStatementMethod\"\n  ],\n  \"\
  $schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MemberProfile\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-member-profile-schema.json
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
title: MemberProfile
---
