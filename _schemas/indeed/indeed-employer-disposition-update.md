---
description: An update to the disposition (application status) of a candidate for a specific job posting. Used to sync hiring pipeline status changes back to Indeed.
layout: schema
name: DispositionUpdate
properties_list:
- description: The unique identifier for the application.
  name: applicationId
  type: string
- description: The new disposition status for the application. Must be one of Indeed's predefined categories.
  name: status
  type: string
- description: The timestamp when the status change occurred.
  name: statusUpdatedAt
  type: string
- description: The reason for rejection, if the status is REJECTED.
  name: rejectionReason
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-disposition-update-schema.json
slug: indeed-employer-disposition-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DispositionUpdate\",\n  \"type\": \"object\",\n  \"description\": \"An update to the disposition (application status) of a candidate for a specific job posting. Used to sync hiring pipeline status changes back to Indeed.\",\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the application.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The new disposition status for the application. Must be one of Indeed's predefined categories.\"\n    },\n    \"statusUpdatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the status change occurred.\"\n    },\n    \"rejectionReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason for rejection, if the status is REJECTED.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-disposition-update-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: DispositionUpdate
---
