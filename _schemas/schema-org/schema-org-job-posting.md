---
description: A listing that describes a job opening in a certain organization.
layout: schema
name: Schema.org JobPosting
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The title of the job.
  name: title
  type: string
- description: A description of the job posting.
  name: description
  type: string
- description: Publication date of an online listing.
  name: datePosted
  type: string
- description: The date after when the listing is not valid.
  name: validThrough
  type: string
- description: URL of the job posting.
  name: url
  type: string
- description: Organization offering the job position.
  name: hiringOrganization
  type: object
- description: A (typically single) geographic location associated with the job position.
  name: jobLocation
  type: object
- description: The location(s) applicants can have their workplace.
  name: applicantLocationRequirements
  type: object
- description: A description of the job location (e.g., TELECOMMUTE for telecommute jobs).
  name: jobLocationType
  type: string
- description: Type of employment.
  name: employmentType
  type: object
- description: The base salary of the job.
  name: baseSalary
  type: object
- description: Educational background needed for the position.
  name: educationRequirements
  type: object
- description: Description of skills and experience needed for the position.
  name: experienceRequirements
  type: string
- description: Specific qualifications required for this role.
  name: qualifications
  type: string
- description: Responsibilities associated with this role.
  name: responsibilities
  type: string
- description: A statement of knowledge, skill, ability, task or any other assertion expressing a competency.
  name: skills
  type: object
- description: The industry associated with the job position.
  name: industry
  type: string
- description: A category describing the job, preferably using a BLS O*NET-SOC taxonomy.
  name: occupationalCategory
  type: string
- description: The typical working hours for this job.
  name: workHours
  type: string
- description: Description of benefits associated with the job.
  name: jobBenefits
  type: string
- description: Description of bonus and commission compensation aspects of the job.
  name: incentiveCompensation
  type: string
- description: Indicates whether an url that is set as the listing for this job goes directly to the site of the business.
  name: directApply
  type: boolean
- description: The identifier property represents any kind of identifier.
  name: identifier
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-job-posting-schema.json
slug: schema-org-job-posting
source_filename: schema-org-job-posting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/job-posting.json\",\n  \"title\": \"Schema.org JobPosting\",\n  \"description\": \"A listing that describes a job opening in a certain organization.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"title\", \"datePosted\", \"description\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"JobPosting\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the job.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the job posting.\"\n    },\n    \"datePosted\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Publication date of an online listing.\"\
  \n    },\n    \"validThrough\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date after when the listing is not valid.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the job posting.\"\n    },\n    \"hiringOrganization\": {\n      \"$ref\": \"schema-org-organization-schema.json\",\n      \"description\": \"Organization offering the job position.\"\n    },\n    \"jobLocation\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-place-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-place-schema.json\" } }\n      ],\n      \"description\": \"A (typically single) geographic location associated with the job position.\"\n    },\n    \"applicantLocationRequirements\": {\n      \"type\": \"object\",\n      \"description\": \"The location(s) applicants can have their workplace.\",\n      \"properties\": {\n        \"@type\": { \"type\"\
  : \"string\", \"const\": \"Country\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"jobLocationType\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the job location (e.g., TELECOMMUTE for telecommute jobs).\"\n    },\n    \"employmentType\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"enum\": [\"FULL_TIME\", \"PART_TIME\", \"CONTRACTOR\", \"TEMPORARY\", \"INTERN\", \"VOLUNTEER\", \"PER_DIEM\", \"OTHER\"] },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Type of employment.\"\n    },\n    \"baseSalary\": {\n      \"type\": \"object\",\n      \"description\": \"The base salary of the job.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MonetaryAmount\" },\n        \"currency\": { \"type\": \"string\", \"pattern\": \"^[A-Z]{3}$\" },\n        \"value\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"\
  @type\": { \"type\": \"string\", \"const\": \"QuantitativeValue\" },\n            \"value\": { \"type\": \"number\" },\n            \"minValue\": { \"type\": \"number\" },\n            \"maxValue\": { \"type\": \"number\" },\n            \"unitText\": { \"type\": \"string\", \"enum\": [\"HOUR\", \"DAY\", \"WEEK\", \"MONTH\", \"YEAR\"] }\n          }\n        }\n      }\n    },\n    \"educationRequirements\": {\n      \"type\": \"object\",\n      \"description\": \"Educational background needed for the position.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"EducationalOccupationalCredential\" },\n        \"credentialCategory\": { \"type\": \"string\" }\n      }\n    },\n    \"experienceRequirements\": {\n      \"type\": \"string\",\n      \"description\": \"Description of skills and experience needed for the position.\"\n    },\n    \"qualifications\": {\n      \"type\": \"string\",\n      \"description\": \"Specific qualifications required for this\
  \ role.\"\n    },\n    \"responsibilities\": {\n      \"type\": \"string\",\n      \"description\": \"Responsibilities associated with this role.\"\n    },\n    \"skills\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"A statement of knowledge, skill, ability, task or any other assertion expressing a competency.\"\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"The industry associated with the job position.\"\n    },\n    \"occupationalCategory\": {\n      \"type\": \"string\",\n      \"description\": \"A category describing the job, preferably using a BLS O*NET-SOC taxonomy.\"\n    },\n    \"workHours\": {\n      \"type\": \"string\",\n      \"description\": \"The typical working hours for this job.\"\n    },\n    \"jobBenefits\": {\n      \"type\": \"string\",\n      \"description\": \"Description of benefits associated with the job.\"\
  \n    },\n    \"incentiveCompensation\": {\n      \"type\": \"string\",\n      \"description\": \"Description of bonus and commission compensation aspects of the job.\"\n    },\n    \"directApply\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether an url that is set as the listing for this job goes directly to the site of the business.\"\n    },\n    \"identifier\": {\n      \"$ref\": \"schema-org-property-value-schema.json\",\n      \"description\": \"The identifier property represents any kind of identifier.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-job-posting-schema.json
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
title: Schema.org JobPosting
---
