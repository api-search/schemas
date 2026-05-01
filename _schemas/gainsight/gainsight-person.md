---
description: Represents a person (contact) record in Gainsight CS, tracking customer stakeholders, their roles, and engagement data.
layout: schema
name: Gainsight Person
properties_list:
- description: Gainsight unique identifier for the person record
  name: Gsid
  type: string
- description: First name
  name: FirstName
  type: string
- description: Last name
  name: LastName
  type: string
- description: Email address
  name: Email
  type: string
- description: Associated company Gsid
  name: CompanyId
  type: string
- description: Associated company name
  name: CompanyName
  type: string
- description: Job title
  name: Title
  type: string
- description: Contact role (e.g., Decision Maker, Champion, End User)
  name: Role
  type: string
- description: Phone number
  name: Phone
  type: string
- description: Location
  name: Location
  type: string
- description: LinkedIn profile URL
  name: LinkedinUrl
  type: string
- description: Timezone
  name: Timezone
  type: string
- description: Linked Salesforce contact ID
  name: SfdcContactId
  type: string
- description: Net Promoter Score
  name: NPS
  type: number
- description: Whether this is the primary contact for the company
  name: IsPrimary
  type: boolean
- description: Whether the person record is active
  name: IsActive
  type: boolean
- description: Record creation timestamp
  name: CreatedDate
  type: string
- description: Record last modification timestamp
  name: ModifiedDate
  type: string
provider_name: Gainsight
provider_slug: gainsight
schema_file: json-schema/gainsight-person-schema.json
slug: gainsight-person
source_filename: gainsight-person-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.gainsight.com/schemas/gainsight/person.json\",\n  \"title\": \"Gainsight Person\",\n  \"description\": \"Represents a person (contact) record in Gainsight CS, tracking customer stakeholders, their roles, and engagement data.\",\n  \"type\": \"object\",\n  \"required\": [\"Email\"],\n  \"properties\": {\n    \"Gsid\": {\n      \"type\": \"string\",\n      \"description\": \"Gainsight unique identifier for the person record\"\n    },\n    \"FirstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name\",\n      \"maxLength\": 128\n    },\n    \"LastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name\",\n      \"maxLength\": 128\n    },\n    \"Email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address\"\n    },\n    \"CompanyId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated\
  \ company Gsid\"\n    },\n    \"CompanyName\": {\n      \"type\": \"string\",\n      \"description\": \"Associated company name\"\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title\"\n    },\n    \"Role\": {\n      \"type\": \"string\",\n      \"description\": \"Contact role (e.g., Decision Maker, Champion, End User)\"\n    },\n    \"Phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number\"\n    },\n    \"Location\": {\n      \"type\": \"string\",\n      \"description\": \"Location\"\n    },\n    \"LinkedinUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"LinkedIn profile URL\"\n    },\n    \"Timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone\"\n    },\n    \"SfdcContactId\": {\n      \"type\": \"string\",\n      \"description\": \"Linked Salesforce contact ID\"\n    },\n    \"NPS\": {\n      \"type\": \"number\",\n      \"description\": \"Net Promoter Score\"\
  ,\n      \"minimum\": -100,\n      \"maximum\": 100\n    },\n    \"IsPrimary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary contact for the company\"\n    },\n    \"IsActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the person record is active\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"ModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last modification timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/json-schema/gainsight-person-schema.json
tags: []
title: Gainsight Person
---
