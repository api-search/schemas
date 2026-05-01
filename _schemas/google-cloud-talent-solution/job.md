---
description: A job posting resource in Google Cloud Talent Solution representing an employment opportunity.
layout: schema
name: Job
properties_list:
- description: Resource name of the job, in the format projects/{projectId}/tenants/{tenantId}/jobs/{jobId}.
  name: name
  type: string
- description: Resource name of the company listing the job.
  name: company
  type: string
- description: Title of the job, such as Software Engineer.
  name: title
  type: string
- description: Description of the job in HTML format.
  name: description
  type: string
- description: Addresses where the job is located.
  name: addresses
  type: array
- description: The employment type(s) of the job.
  name: employmentTypes
  type: array
- description: Job compensation information.
  name: compensationInfo
  type: object
- description: A description of job qualifications.
  name: qualifications
  type: string
- description: A description of job responsibilities.
  name: responsibilities
  type: string
- description: The job posting region.
  name: postingRegion
  type: string
- description: Timestamp when the job posting expires.
  name: postingExpireTime
  type: string
- description: Timestamp when the job posting was created.
  name: postingCreateTime
  type: string
- description: Timestamp when the job posting was last updated.
  name: postingUpdateTime
  type: string
- description: The language of the posting, such as en-US.
  name: languageCode
  type: string
provider_name: Google Cloud Talent Solution
provider_slug: google-cloud-talent-solution
schema_file: json-schema/job.json
slug: job
source_filename: job.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-talent-solution/refs/heads/main/json-schema/job.json\",\n  \"title\": \"Job\",\n  \"description\": \"A job posting resource in Google Cloud Talent Solution representing an employment opportunity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the job, in the format projects/{projectId}/tenants/{tenantId}/jobs/{jobId}.\"\n    },\n    \"company\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name of the company listing the job.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the job, such as Software Engineer.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the job in HTML format.\"\n    },\n    \"addresses\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Addresses where the job is located.\"\n    },\n    \"employmentTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"EMPLOYMENT_TYPE_UNSPECIFIED\",\n          \"FULL_TIME\",\n          \"PART_TIME\",\n          \"CONTRACTOR\",\n          \"CONTRACT_TO_HIRE\",\n          \"TEMPORARY\",\n          \"INTERN\",\n          \"VOLUNTEER\",\n          \"PER_DIEM\",\n          \"OTHER\"\n        ]\n      },\n      \"description\": \"The employment type(s) of the job.\"\n    },\n    \"compensationInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Job compensation information.\",\n      \"properties\": {\n        \"entries\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n  \
  \              \"description\": \"Compensation type.\"\n              },\n              \"unit\": {\n                \"type\": \"string\",\n                \"description\": \"Frequency of the compensation.\"\n              },\n              \"amount\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"currencyCode\": {\n                    \"type\": \"string\"\n                  },\n                  \"units\": {\n                    \"type\": \"string\"\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"qualifications\": {\n      \"type\": \"string\",\n      \"description\": \"A description of job qualifications.\"\n    },\n    \"responsibilities\": {\n      \"type\": \"string\",\n      \"description\": \"A description of job responsibilities.\"\n    },\n    \"postingRegion\": {\n      \"type\": \"string\",\n      \"description\": \"The job posting region.\"\n    },\n  \
  \  \"postingExpireTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job posting expires.\"\n    },\n    \"postingCreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job posting was created.\"\n    },\n    \"postingUpdateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the job posting was last updated.\"\n    },\n    \"languageCode\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the posting, such as en-US.\"\n    }\n  },\n  \"required\": [\"company\", \"title\", \"description\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-talent-solution/refs/heads/main/json-schema/job.json
tags:
- Google Cloud
- Jobs
- Machine Learning
- Recruitment
- Search
- Talent
title: Job
---
