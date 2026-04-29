---
description: PeopleSoft Campus Solutions student record.
layout: schema
name: Student
properties_list:
- description: Student ID.
  name: EMPLID
  type: string
- description: Student name.
  name: NAME
  type: string
- description: Academic career.
  name: ACAD_CAREER
  type: string
- description: Academic program.
  name: ACAD_PROG
  type: string
- description: Academic plan/major.
  name: ACAD_PLAN
  type: string
- description: Admission term.
  name: ADMIT_TERM
  type: string
- description: Academic level.
  name: ACAD_LEVEL_BOT
  type: string
- description: Cumulative GPA.
  name: CUM_GPA
  type: number
- description: Total GPA units taken.
  name: TOT_TAKEN_GPA
  type: number
- description: Institution code.
  name: INSTITUTION
  type: string
- description: Campus code.
  name: CAMPUS
  type: string
- description: Student career number.
  name: STDNT_CAR_NBR
  type: integer
- description: Academic standing.
  name: ACAD_STANDING
  type: string
provider_name: PeopleSoft
provider_slug: peoplesoft
schema_file: json-schema/peoplesoft-campus-solutions-student-schema.json
slug: peoplesoft-campus-solutions-student
source_filename: peoplesoft-campus-solutions-student-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-campus-solutions-student-schema.json\",\n  \"title\": \"Student\",\n  \"description\": \"PeopleSoft Campus Solutions student record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMPLID\": {\n      \"type\": \"string\",\n      \"description\": \"Student ID.\",\n      \"example\": \"STU001234\"\n    },\n    \"NAME\": {\n      \"type\": \"string\",\n      \"description\": \"Student name.\",\n      \"example\": \"Alex Johnson\"\n    },\n    \"ACAD_CAREER\": {\n      \"type\": \"string\",\n      \"description\": \"Academic career.\",\n      \"enum\": [\n        \"UGRD\",\n        \"GRAD\",\n        \"LAW\",\n        \"MED\"\n      ],\n      \"example\": \"UGRD\"\n    },\n    \"ACAD_PROG\": {\n      \"type\": \"string\",\n      \"description\": \"Academic program.\",\n      \"example\": \"BSCS\"\
  \n    },\n    \"ACAD_PLAN\": {\n      \"type\": \"string\",\n      \"description\": \"Academic plan/major.\",\n      \"example\": \"COMPSCI\"\n    },\n    \"ADMIT_TERM\": {\n      \"type\": \"string\",\n      \"description\": \"Admission term.\",\n      \"example\": \"2026F\"\n    },\n    \"ACAD_LEVEL_BOT\": {\n      \"type\": \"string\",\n      \"description\": \"Academic level.\",\n      \"enum\": [\n        \"FR\",\n        \"SO\",\n        \"JR\",\n        \"SR\",\n        \"GR\"\n      ],\n      \"example\": \"JR\"\n    },\n    \"CUM_GPA\": {\n      \"type\": \"number\",\n      \"description\": \"Cumulative GPA.\",\n      \"example\": 3.65\n    },\n    \"TOT_TAKEN_GPA\": {\n      \"type\": \"number\",\n      \"description\": \"Total GPA units taken.\",\n      \"example\": 90.0\n    },\n    \"INSTITUTION\": {\n      \"type\": \"string\",\n      \"description\": \"Institution code.\",\n      \"example\": \"MYUNV\"\n    },\n    \"CAMPUS\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Campus code.\",\n      \"example\": \"MAIN\"\n    },\n    \"STDNT_CAR_NBR\": {\n      \"type\": \"integer\",\n      \"description\": \"Student career number.\",\n      \"example\": 0\n    },\n    \"ACAD_STANDING\": {\n      \"type\": \"string\",\n      \"description\": \"Academic standing.\",\n      \"enum\": [\n        \"GS\",\n        \"GP\",\n        \"AP\",\n        \"DQ\"\n      ],\n      \"example\": \"GS\"\n    }\n  },\n  \"x-schema-source\": \"domain-knowledge\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-campus-solutions-student-schema.json
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
title: Student
---
