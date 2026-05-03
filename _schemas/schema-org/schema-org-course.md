---
description: A description of an educational course which may be offered as distinct instances which take place at different times or locations, or through different media.
layout: schema
name: Schema.org Course
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the course.
  name: name
  type: string
- description: A description of the course.
  name: description
  type: string
- description: URL of the course.
  name: url
  type: string
- description: An image of the course.
  name: image
  type: object
- description: The service provider of the course.
  name: provider
  type: object
- description: The identifier for the Course used by the course provider.
  name: courseCode
  type: string
- description: Requirements for taking the course.
  name: coursePrerequisites
  type: object
- description: The level in terms of progression through an educational or training context.
  name: educationalLevel
  type: string
- description: A description of the qualification or credential awarded upon completion.
  name: educationalCredentialAwarded
  type: string
- description: The number of credits or units awarded by a Course.
  name: numberOfCredits
  type: object
- description: An offering of the course at a specific time and place.
  name: hasCourseInstance
  type: object
- description: The subject matter of the course.
  name: about
  type: object
- description: The language of the course content.
  name: inLanguage
  type: string
- description: The item being described is intended to help a person learn the competency or learning outcome.
  name: teaches
  type: object
- description: The total number of students that have enrolled in the history of the course.
  name: totalHistoricalEnrollment
  type: integer
- description: A financial aid type or program which students may use to pay for the course.
  name: financialAidEligible
  type: string
- description: A language someone may use with or at the item.
  name: availableLanguage
  type: object
- description: The overall rating.
  name: aggregateRating
  type: object
- description: A review of the course.
  name: review
  type: object
- description: An offer to provide this course.
  name: offers
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-course-schema.json
slug: schema-org-course
source_filename: schema-org-course-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/course.json\",\n  \"title\": \"Schema.org Course\",\n  \"description\": \"A description of an educational course which may be offered as distinct instances which take place at different times or locations, or through different media.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"Course\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the course.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the course.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\":\
  \ \"URL of the course.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the course.\"\n    },\n    \"provider\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The service provider of the course.\"\n    },\n    \"courseCode\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the Course used by the course provider.\"\n    },\n    \"coursePrerequisites\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"oneOf\": [{ \"type\": \"string\" }, { \"$ref\": \"#\" }] } }\n      ],\n      \"description\": \"Requirements for taking the course.\"\n    },\n    \"educationalLevel\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The level in terms of progression through an educational or training context.\"\n    },\n    \"educationalCredentialAwarded\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the qualification or credential awarded upon completion.\"\n    },\n    \"numberOfCredits\": {\n      \"oneOf\": [\n        { \"type\": \"integer\" },\n        { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"StructuredValue\" }, \"value\": { \"type\": \"integer\" } } }\n      ],\n      \"description\": \"The number of credits or units awarded by a Course.\"\n    },\n    \"hasCourseInstance\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/CourseInstance\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/CourseInstance\" } }\n      ],\n      \"description\": \"An offering of the course at a specific time and place.\"\n    },\n    \"about\": {\n      \"type\": \"object\",\n      \"description\": \"The subject\
  \ matter of the course.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"inLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the course content.\"\n    },\n    \"teaches\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"The item being described is intended to help a person learn the competency or learning outcome.\"\n    },\n    \"totalHistoricalEnrollment\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of students that have enrolled in the history of the course.\"\n    },\n    \"financialAidEligible\": {\n      \"type\": \"string\",\n      \"description\": \"A financial aid type or program which students may use to pay for the course.\"\n    },\n    \"availableLanguage\": {\n      \"oneOf\": [\n        { \"type\": \"\
  string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"A language someone may use with or at the item.\"\n    },\n    \"aggregateRating\": {\n      \"$ref\": \"schema-org-aggregate-rating-schema.json\",\n      \"description\": \"The overall rating.\"\n    },\n    \"review\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-review-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-review-schema.json\" } }\n      ],\n      \"description\": \"A review of the course.\"\n    },\n    \"offers\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-offer-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-offer-schema.json\" } }\n      ],\n      \"description\": \"An offer to provide this course.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"\
  string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  },\n  \"$defs\": {\n    \"CourseInstance\": {\n      \"type\": \"object\",\n      \"description\": \"An instance of a Course offered at a specific time and place.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"CourseInstance\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the course instance.\" },\n        \"courseMode\": { \"type\": \"string\", \"description\": \"The medium or means of delivery of the course instance (e.g., online, onsite, blended).\" },\n        \"courseWorkload\": { \"type\": \"string\", \"description\": \"The amount of work expected of students.\" },\n        \"instructor\": { \"$ref\": \"schema-org-person-schema.json\", \"description\": \"A person assigned to instruct or provide educational instruction.\" },\n        \"startDate\": { \"type\"\
  : \"string\", \"format\": \"date\", \"description\": \"The start date.\" },\n        \"endDate\": { \"type\": \"string\", \"format\": \"date\", \"description\": \"The end date.\" },\n        \"location\": { \"oneOf\": [{ \"type\": \"string\" }, { \"$ref\": \"schema-org-place-schema.json\" }], \"description\": \"The location of the course instance.\" },\n        \"courseSchedule\": { \"type\": \"object\", \"description\": \"Represents the schedule for the course.\", \"properties\": { \"@type\": { \"const\": \"Schedule\" }, \"repeatFrequency\": { \"type\": \"string\" }, \"repeatCount\": { \"type\": \"integer\" } } }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-course-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org Course
---
