---
description: ''
layout: schema
name: sasbScoresAll
properties_list:
- description: Date for the period requested expressed in YYYY-MM-DD format.
  name: date
  type: string
- description: FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).
  name: fsymId
  type: string
- description: Identifier that was used for the request.
  name: requestId
  type: string
- description: 'The name of the specific SASB Score type being shown in the response. This will be represented by the scoreTypes input: PULSE, INSIGHT, MOMENTUM, ART_VOL_TTM, CAT_VOL_TTM, or DYNAMIC_MAT.'
  name: scoreType
  type: string
- description: The Access and Affordability SASB Category.
  name: accessAndAffordability
  type: number
- description: The Air Quality SASB Category.
  name: airQuality
  type: number
- description: The All Categories Category. This represents the overall SASB Score for the given 'scoreType'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double
  name: allCategories
  type: object
- description: The Business Ethics Category.
  name: businessEthics
  type: number
- description: The Business Model Resilience Category.
  name: businessModelResilience
  type: number
- description: The Competitive Behavior Category.
  name: competitiveBehavior
  type: number
- description: The Critical Incident Risk Management Category.
  name: criticalIncidentRiskManagement
  type: number
- description: The Customer Privacy Category.
  name: customerPrivacy
  type: number
- description: The Customer Welfare Category.
  name: customerWelfare
  type: number
- description: The Data Security Category.
  name: dataSecurity
  type: number
- description: The Ecological Impacts Category.
  name: ecologicalImpacts
  type: number
- description: The Employee Engagement Diversity and Inclusion Category.
  name: employeeEngagementDiversityandInclusion
  type: number
- description: The Employee Health And Safety Category.
  name: employeeHealthAndSafety
  type: number
- description: The Energy Management Category.
  name: energyManagement
  type: number
- description: The Greenhouse Gases Emissions Category.
  name: gHGEmissions
  type: number
- description: The Human Rights and Community Relations Category.
  name: humanRightsandCommunityRelations
  type: number
- description: The Labor Practices Category.
  name: laborPractices
  type: number
- description: The Management of the Legal and Regulatory Environment Category.
  name: managementOfTheLegalAndRegulatoryEnvironment
  type: number
- description: The Materials Sourcing and Efficiency Category.
  name: materialsSourcingAndEfficiency
  type: number
- description: The Materiality Category. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.
  name: materiality
  type: object
- description: The Physical Impacts of Climate Change Category.
  name: physicalImpactsOfClimateChange
  type: number
- description: The Product Quality and Safety Category.
  name: productQualityAndSafety
  type: number
- description: The Product Design And Lifecycle Management Category.
  name: productDesignAndLifecycleManagement
  type: number
- description: The Selling Practices And Product Labeling Category.
  name: sellingPracticesAndProductLabeling
  type: number
- description: The Supply Chain Management Category.
  name: supplyChainManagement
  type: number
- description: The Systemic Risk Management Category.
  name: systemicRiskManagement
  type: number
- description: The Waste and Hazardous Materials Management Category.
  name: wasteAndHazardousMaterialsManagement
  type: number
- description: The Water and Wastewater Management Category.
  name: waterAndWastewaterManagement
  type: number
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-esg-sasb-scores-all-schema.json
slug: factset-esg-sasb-scores-all
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"sasbScoresAll\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"description\": \"Date for the period requested expressed in YYYY-MM-DD format.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    },\n    \"scoreType\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the specific SASB Score type being shown in the response. This will be represented by the scoreTypes input: PULSE, INSIGHT, MOMENTUM, ART_VOL_TTM, CAT_VOL_TTM, or DYNAMIC_MAT.\"\n    },\n    \"accessAndAffordability\": {\n      \"type\": \"number\",\n      \"description\": \"The Access and\
  \ Affordability SASB Category.\"\n    },\n    \"airQuality\": {\n      \"type\": \"number\",\n      \"description\": \"The Air Quality SASB Category.\"\n    },\n    \"allCategories\": {\n      \"type\": \"object\",\n      \"description\": \"The All Categories Category. This represents the overall SASB Score for the given 'scoreType'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.\"\n    },\n    \"businessEthics\": {\n      \"type\": \"number\",\n      \"description\": \"The Business Ethics Category.\"\n    },\n    \"businessModelResilience\": {\n      \"type\": \"number\",\n      \"description\": \"The Business Model Resilience Category.\"\n    },\n    \"competitiveBehavior\": {\n      \"type\": \"number\",\n      \"description\": \"The Competitive Behavior Category.\"\n    },\n    \"criticalIncidentRiskManagement\": {\n      \"type\": \"number\",\n      \"description\": \"The Critical Incident Risk Management Category.\"\
  \n    },\n    \"customerPrivacy\": {\n      \"type\": \"number\",\n      \"description\": \"The Customer Privacy Category.\"\n    },\n    \"customerWelfare\": {\n      \"type\": \"number\",\n      \"description\": \"The Customer Welfare Category.\"\n    },\n    \"dataSecurity\": {\n      \"type\": \"number\",\n      \"description\": \"The Data Security Category.\"\n    },\n    \"ecologicalImpacts\": {\n      \"type\": \"number\",\n      \"description\": \"The Ecological Impacts Category.\"\n    },\n    \"employeeEngagementDiversityandInclusion\": {\n      \"type\": \"number\",\n      \"description\": \"The Employee Engagement Diversity and Inclusion Category.\"\n    },\n    \"employeeHealthAndSafety\": {\n      \"type\": \"number\",\n      \"description\": \"The Employee Health And Safety Category.\"\n    },\n    \"energyManagement\": {\n      \"type\": \"number\",\n      \"description\": \"The Energy Management Category.\"\n    },\n    \"gHGEmissions\": {\n      \"type\": \"number\",\n\
  \      \"description\": \"The Greenhouse Gases Emissions Category.\"\n    },\n    \"humanRightsandCommunityRelations\": {\n      \"type\": \"number\",\n      \"description\": \"The Human Rights and Community Relations Category.\"\n    },\n    \"laborPractices\": {\n      \"type\": \"number\",\n      \"description\": \"The Labor Practices Category.\"\n    },\n    \"managementOfTheLegalAndRegulatoryEnvironment\": {\n      \"type\": \"number\",\n      \"description\": \"The Management of the Legal and Regulatory Environment Category.\"\n    },\n    \"materialsSourcingAndEfficiency\": {\n      \"type\": \"number\",\n      \"description\": \"The Materials Sourcing and Efficiency Category.\"\n    },\n    \"materiality\": {\n      \"type\": \"object\",\n      \"description\": \"The Materiality Category. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.\"\n    },\n    \"physicalImpactsOfClimateChange\": {\n      \"type\": \"number\"\
  ,\n      \"description\": \"The Physical Impacts of Climate Change Category.\"\n    },\n    \"productQualityAndSafety\": {\n      \"type\": \"number\",\n      \"description\": \"The Product Quality and Safety Category.\"\n    },\n    \"productDesignAndLifecycleManagement\": {\n      \"type\": \"number\",\n      \"description\": \"The Product Design And Lifecycle Management Category.\"\n    },\n    \"sellingPracticesAndProductLabeling\": {\n      \"type\": \"number\",\n      \"description\": \"The Selling Practices And Product Labeling Category.\"\n    },\n    \"supplyChainManagement\": {\n      \"type\": \"number\",\n      \"description\": \"The Supply Chain Management Category.\"\n    },\n    \"systemicRiskManagement\": {\n      \"type\": \"number\",\n      \"description\": \"The Systemic Risk Management Category.\"\n    },\n    \"wasteAndHazardousMaterialsManagement\": {\n      \"type\": \"number\",\n      \"description\": \"The Waste and Hazardous Materials Management Category.\"\n\
  \    },\n    \"waterAndWastewaterManagement\": {\n      \"type\": \"number\",\n      \"description\": \"The Water and Wastewater Management Category.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-esg-sasb-scores-all-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: sasbScoresAll
---
