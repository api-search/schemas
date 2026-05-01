---
description: Represents a company record in Gainsight CS, the primary account object for tracking customer success relationships, health scores, and revenue metrics.
layout: schema
name: Gainsight Company
properties_list:
- description: Gainsight unique identifier for the company record
  name: Gsid
  type: string
- description: Company name
  name: Name
  type: string
- description: Industry classification
  name: Industry
  type: string
- description: Annual recurring revenue
  name: ARR
  type: number
- description: Monthly recurring revenue
  name: MRR
  type: number
- description: Current customer lifecycle stage
  name: LifecycleStage
  type: string
- description: Company stage
  name: Stage
  type: string
- description: Company status (e.g., Active, Churned)
  name: Status
  type: string
- description: Name of the assigned Customer Success Manager
  name: CSMName
  type: string
- description: Number of employees
  name: Employees
  type: integer
- description: Original contract start date
  name: OriginalContractDate
  type: string
- description: Next renewal date
  name: RenewalDate
  type: string
- description: Overall health score value
  name: OverallScore
  type: number
- description: Current health score identifier
  name: CurrScoreId
  type: string
- description: Linked Salesforce account ID
  name: SfdcAccountId
  type: string
- description: Parent company Gsid for hierarchical relationships
  name: ParentCompanyId
  type: string
- description: Record creation timestamp
  name: CreatedDate
  type: string
- description: Record last modification timestamp
  name: ModifiedDate
  type: string
provider_name: Gainsight
provider_slug: gainsight
schema_file: json-schema/gainsight-company-schema.json
slug: gainsight-company
source_filename: gainsight-company-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.gainsight.com/schemas/gainsight/company.json\",\n  \"title\": \"Gainsight Company\",\n  \"description\": \"Represents a company record in Gainsight CS, the primary account object for tracking customer success relationships, health scores, and revenue metrics.\",\n  \"type\": \"object\",\n  \"required\": [\"Name\"],\n  \"properties\": {\n    \"Gsid\": {\n      \"type\": \"string\",\n      \"description\": \"Gainsight unique identifier for the company record\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Company name\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"Industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry classification\"\n    },\n    \"ARR\": {\n      \"type\": \"number\",\n      \"description\": \"Annual recurring revenue\",\n      \"minimum\": 0\n    },\n    \"MRR\": {\n      \"type\": \"number\"\
  ,\n      \"description\": \"Monthly recurring revenue\",\n      \"minimum\": 0\n    },\n    \"LifecycleStage\": {\n      \"type\": \"string\",\n      \"description\": \"Current customer lifecycle stage\"\n    },\n    \"Stage\": {\n      \"type\": \"string\",\n      \"description\": \"Company stage\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Company status (e.g., Active, Churned)\"\n    },\n    \"CSMName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the assigned Customer Success Manager\"\n    },\n    \"Employees\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of employees\",\n      \"minimum\": 0\n    },\n    \"OriginalContractDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Original contract start date\"\n    },\n    \"RenewalDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Next renewal date\"\n    },\n    \"OverallScore\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Overall health score value\"\n    },\n    \"CurrScoreId\": {\n      \"type\": \"string\",\n      \"description\": \"Current health score identifier\"\n    },\n    \"SfdcAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Linked Salesforce account ID\"\n    },\n    \"ParentCompanyId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent company Gsid for hierarchical relationships\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"ModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last modification timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/json-schema/gainsight-company-schema.json
tags: []
title: Gainsight Company
---
