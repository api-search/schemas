---
description: PeopleSoft class enrollment record.
layout: schema
name: ClassEnrollment
properties_list:
- description: Student ID.
  name: EMPLID
  type: string
- description: Class number.
  name: CLASS_NBR
  type: integer
- description: Course ID.
  name: CRSE_ID
  type: string
- description: Subject area.
  name: SUBJECT
  type: string
- description: Catalog number.
  name: CATALOG_NBR
  type: string
- description: Course description.
  name: DESCR
  type: string
- description: Units taken.
  name: UNT_TAKEN
  type: number
- description: Grade.
  name: GRADE_INPUT
  type: string
- description: Enrollment status.
  name: ENRL_STATUS_REASON
  type: string
- description: Term code.
  name: STRM
  type: string
provider_name: PeopleSoft
provider_slug: peoplesoft
schema_file: json-schema/peoplesoft-campus-solutions-class-enrollment-schema.json
slug: peoplesoft-campus-solutions-class-enrollment
source_filename: peoplesoft-campus-solutions-class-enrollment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-campus-solutions-class-enrollment-schema.json\",\n  \"title\": \"ClassEnrollment\",\n  \"description\": \"PeopleSoft class enrollment record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMPLID\": {\n      \"type\": \"string\",\n      \"description\": \"Student ID.\",\n      \"example\": \"STU001234\"\n    },\n    \"CLASS_NBR\": {\n      \"type\": \"integer\",\n      \"description\": \"Class number.\",\n      \"example\": 10542\n    },\n    \"CRSE_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Course ID.\",\n      \"example\": \"CS101\"\n    },\n    \"SUBJECT\": {\n      \"type\": \"string\",\n      \"description\": \"Subject area.\",\n      \"example\": \"COMPSCI\"\n    },\n    \"CATALOG_NBR\": {\n      \"type\": \"string\",\n      \"description\": \"Catalog number.\"\
  ,\n      \"example\": \"101\"\n    },\n    \"DESCR\": {\n      \"type\": \"string\",\n      \"description\": \"Course description.\",\n      \"example\": \"Introduction to Computer Science\"\n    },\n    \"UNT_TAKEN\": {\n      \"type\": \"number\",\n      \"description\": \"Units taken.\",\n      \"example\": 3.0\n    },\n    \"GRADE_INPUT\": {\n      \"type\": \"string\",\n      \"description\": \"Grade.\",\n      \"example\": \"A\"\n    },\n    \"ENRL_STATUS_REASON\": {\n      \"type\": \"string\",\n      \"description\": \"Enrollment status.\",\n      \"enum\": [\n        \"ENRL\",\n        \"DROP\",\n        \"WAIT\"\n      ],\n      \"example\": \"ENRL\"\n    },\n    \"STRM\": {\n      \"type\": \"string\",\n      \"description\": \"Term code.\",\n      \"example\": \"2261\"\n    }\n  },\n  \"x-schema-source\": \"domain-knowledge\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-campus-solutions-class-enrollment-schema.json
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
title: ClassEnrollment
---
