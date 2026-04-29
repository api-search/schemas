---
description: Individual job posting element
layout: schema
name: JobPostingElement
properties_list:
- description: External identifier for the job posting
  name: externalJobPostingId
  type: string
- description: Job title
  name: title
  type: string
- description: Full job description
  name: description
  type: string
- description: Organization URN for the job posting
  name: integrationContext
  type: string
- description: Operation type for the job posting
  name: jobPostingOperationType
  type: string
- description: Type of job listing
  name: listingType
  type: string
- description: Timestamp when the job was listed
  name: listedAt
  type: integer
- description: Job location
  name: location
  type: string
- description: URL for company's application page
  name: companyApplyUrl
  type: string
- description: ''
  name: onsiteApplyConfiguration
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-job-posting-element-schema.json
slug: linkedin-talent-job-posting-job-posting-element
source_filename: linkedin-talent-job-posting-job-posting-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-job-posting-element-schema.json\",\n  \"title\": \"JobPostingElement\",\n  \"description\": \"Individual job posting element\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalJobPostingId\": {\n      \"type\": \"string\",\n      \"description\": \"External identifier for the job posting\",\n      \"example\": \"JOB-2024-001\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title\",\n      \"example\": \"Software Developer in Test\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full job description\",\n      \"example\": \"We are looking for a talented Software Developer in Test to join our engineering team...\"\n    },\n    \"integrationContext\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Organization URN for the job posting\",\n      \"example\": \"urn:li:organization:12345678\"\n    },\n    \"jobPostingOperationType\": {\n      \"type\": \"string\",\n      \"description\": \"Operation type for the job posting\",\n      \"enum\": [\n        \"CREATE\",\n        \"UPDATE\",\n        \"CLOSE\"\n      ],\n      \"example\": \"CREATE\"\n    },\n    \"listingType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of job listing\",\n      \"enum\": [\n        \"BASIC\",\n        \"PREMIUM\"\n      ],\n      \"example\": \"BASIC\"\n    },\n    \"listedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Timestamp when the job was listed\",\n      \"example\": 1702693664000\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Job location\",\n      \"example\": \"San Francisco, CA\"\n    },\n    \"companyApplyUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\"\
  : \"URL for company's application page\",\n      \"example\": \"https://company.com/careers/apply\"\n    },\n    \"onsiteApplyConfiguration\": {\n      \"$ref\": \"#/components/schemas/OnsiteApplyConfiguration\"\n    }\n  },\n  \"required\": [\n    \"externalJobPostingId\",\n    \"title\",\n    \"description\",\n    \"integrationContext\",\n    \"listingType\",\n    \"location\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-job-posting-element-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: JobPostingElement
---
