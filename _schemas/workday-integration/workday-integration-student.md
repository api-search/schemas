---
description: Represents a student record within the Workday Student system, including enrollment, academic program, and demographic information.
layout: schema
name: Student
properties_list:
- description: The unique Workday identifier for the student
  name: id
  type: string
- description: The display name of the student
  name: descriptor
  type: string
- description: The student identification number
  name: studentID
  type: string
- description: The academic program the student is enrolled in
  name: academicProgram
  type: object
- description: The academic level (Undergraduate, Graduate, etc.)
  name: academicLevel
  type: object
- description: The current enrollment status
  name: enrollmentStatus
  type: string
- description: The date the student was admitted
  name: admissionDate
  type: string
- description: The expected graduation date
  name: expectedGraduationDate
  type:
  - string
  - 'null'
- description: The cumulative grade point average
  name: gpa
  type: number
- description: The total academic credits earned
  name: totalCreditsEarned
  type: number
provider_name: Workday Integration
provider_slug: workday-integration
schema_file: json-schema/workday-integration-student-schema.json
slug: workday-integration-student
source_filename: workday-integration-student-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.workday.com/student\",\n  \"title\": \"Student\",\n  \"description\": \"Represents a student record within the Workday Student system, including enrollment, academic program, and demographic information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique Workday identifier for the student\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the student\"\n    },\n    \"studentID\": {\n      \"type\": \"string\",\n      \"description\": \"The student identification number\"\n    },\n    \"academicProgram\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The academic program the student is enrolled in\"\n    },\n    \"academicLevel\": {\n      \"$ref\": \"#/$defs/ResourceReference\",\n      \"description\": \"The academic\
  \ level (Undergraduate, Graduate, etc.)\"\n    },\n    \"enrollmentStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current enrollment status\"\n    },\n    \"admissionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the student was admitted\"\n    },\n    \"expectedGraduationDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"The expected graduation date\"\n    },\n    \"gpa\": {\n      \"type\": \"number\",\n      \"description\": \"The cumulative grade point average\"\n    },\n    \"totalCreditsEarned\": {\n      \"type\": \"number\",\n      \"description\": \"The total academic credits earned\"\n    }\n  },\n  \"required\": [\"id\", \"descriptor\"],\n  \"$defs\": {\n    \"ResourceReference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"descriptor\": {\n          \"type\"\
  : \"string\"\n        },\n        \"href\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"id\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integration/refs/heads/main/json-schema/workday-integration-student-schema.json
tags:
- Enterprise
- ERP
- Finance
- HCM
- Integration
- Payroll
title: Student
---
