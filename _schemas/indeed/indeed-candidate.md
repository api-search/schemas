---
description: A candidate object from the Indeed Employer API, representing a job applicant who has applied to a position through Indeed or Indeed Apply. Contains personal details, resume, application status, and responses to screener and EEO questions.
layout: schema
name: Indeed Candidate
properties_list:
- description: A unique candidate application identifier. For Indeed Apply applications, this is a 64-character string (apply_id) that uniquely connects the employer, candidate, and job posting.
  name: id
  type: string
- description: The candidate's full name as provided in their application.
  name: name
  type: string
- description: The candidate's first (given) name.
  name: firstName
  type: string
- description: The candidate's last (family) name.
  name: lastName
  type: string
- description: The candidate's email address.
  name: email
  type: string
- description: The candidate's phone number, typically in E.164 or national format.
  name: phoneNumber
  type: string
- description: The candidate's location as a freeform text string, such as city and state.
  name: location
  type: string
- description: The candidate's resume in multiple formats. Not all formats are always available; use a robust parser that treats missing fields as empty.
  name: resume
  type: object
- description: The candidate's cover letter text, if provided with the application.
  name: coverLetter
  type: string
- description: The current disposition status of the candidate's application within the hiring pipeline. Must map to one of Indeed's six predefined categories.
  name: applicationStatus
  type: string
- description: The candidate's responses to screener questions configured on the job posting.
  name: screenerQuestionResponses
  type: array
- description: Equal Employment Opportunity (EEO) compliance responses provided by the candidate. Only available for US employers that have EEO questions enabled on their job postings.
  name: eeoResponses
  type: object
- description: The ISO 8601 timestamp when the candidate submitted their application.
  name: appliedAt
  type: string
- description: The channel through which the candidate submitted their application, such as indeed_apply, organic, or other integration sources.
  name: source
  type: string
- description: The unique identifier of the job posting the candidate applied to.
  name: jobPostingId
  type: string
- description: The title of the job posting the candidate applied to.
  name: jobTitle
  type: string
- description: The unique identifier of the employer who posted the job.
  name: employerId
  type: string
- description: Whether this candidate application has been acknowledged by the ATS. Unacknowledged applications are returned first in Retrieve Candidates API queries.
  name: acknowledged
  type: boolean
- description: The ISO 8601 timestamp when the candidate record was last updated.
  name: updatedAt
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-candidate-schema.json
slug: indeed-candidate
source_filename: indeed-candidate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-candidate-schema.json\",\n  \"title\": \"Indeed Candidate\",\n  \"description\": \"A candidate object from the Indeed Employer API, representing a job applicant who has applied to a position through Indeed or Indeed Apply. Contains personal details, resume, application status, and responses to screener and EEO questions.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"email\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique candidate application identifier. For Indeed Apply applications, this is a 64-character string (apply_id) that uniquely connects the employer, candidate, and job posting.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's full name as provided in their application.\"\n\
  \    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's first (given) name.\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's last (family) name.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The candidate's email address.\"\n    },\n    \"phoneNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's phone number, typically in E.164 or national format.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's location as a freeform text string, such as city and state.\"\n    },\n    \"resume\": {\n      \"type\": \"object\",\n      \"description\": \"The candidate's resume in multiple formats. Not all formats are always available; use a robust parser that treats missing fields as empty.\",\n      \"properties\": {\n        \"file\": {\n          \"type\":\
  \ \"object\",\n          \"description\": \"The uploaded resume file.\",\n          \"properties\": {\n            \"fileName\": {\n              \"type\": \"string\",\n              \"description\": \"The original filename of the uploaded resume document.\"\n            },\n            \"contentType\": {\n              \"type\": \"string\",\n              \"description\": \"The MIME type of the resume file, such as application/pdf or application/msword.\"\n            },\n            \"data\": {\n              \"type\": \"string\",\n              \"contentEncoding\": \"base64\",\n              \"description\": \"The raw binary content of the resume file, Base64-encoded.\"\n            }\n          }\n        },\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Plain text representation of the resume content.\"\n        },\n        \"html\": {\n          \"type\": \"string\",\n          \"description\": \"HTML-formatted representation of the resume content.\"\
  \n        },\n        \"json\": {\n          \"type\": \"object\",\n          \"description\": \"Structured JSON representation of the parsed resume data from Indeed Resume.\",\n          \"properties\": {\n            \"workExperience\": {\n              \"type\": \"array\",\n              \"description\": \"The candidate's work experience history.\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"title\": {\n                    \"type\": \"string\",\n                    \"description\": \"Job title held by the candidate.\"\n                  },\n                  \"company\": {\n                    \"type\": \"string\",\n                    \"description\": \"Name of the employer or company.\"\n                  },\n                  \"location\": {\n                    \"type\": \"string\",\n                    \"description\": \"Location of the position.\"\n                  },\n                  \"startDate\"\
  : {\n                    \"type\": \"string\",\n                    \"description\": \"Start date of employment.\"\n                  },\n                  \"endDate\": {\n                    \"type\": \"string\",\n                    \"description\": \"End date of employment. Null or absent if currently employed.\"\n                  },\n                  \"current\": {\n                    \"type\": \"boolean\",\n                    \"description\": \"Whether this is the candidate's current position.\"\n                  },\n                  \"description\": {\n                    \"type\": \"string\",\n                    \"description\": \"Description of responsibilities and achievements.\"\n                  }\n                }\n              }\n            },\n            \"education\": {\n              \"type\": \"array\",\n              \"description\": \"The candidate's educational background.\",\n              \"items\": {\n                \"type\": \"object\",\n          \
  \      \"properties\": {\n                  \"institution\": {\n                    \"type\": \"string\",\n                    \"description\": \"Name of the educational institution.\"\n                  },\n                  \"degree\": {\n                    \"type\": \"string\",\n                    \"description\": \"Degree or certification obtained.\"\n                  },\n                  \"fieldOfStudy\": {\n                    \"type\": \"string\",\n                    \"description\": \"Field of study or major.\"\n                  },\n                  \"startDate\": {\n                    \"type\": \"string\",\n                    \"description\": \"Start date of attendance.\"\n                  },\n                  \"endDate\": {\n                    \"type\": \"string\",\n                    \"description\": \"End date or graduation date.\"\n                  },\n                  \"location\": {\n                    \"type\": \"string\",\n                    \"description\"\
  : \"Location of the institution.\"\n                  }\n                }\n              }\n            },\n            \"skills\": {\n              \"type\": \"array\",\n              \"description\": \"List of skills from the candidate's resume.\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"certifications\": {\n              \"type\": \"array\",\n              \"description\": \"Professional certifications held by the candidate.\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"name\": {\n                    \"type\": \"string\",\n                    \"description\": \"Name of the certification.\"\n                  },\n                  \"issuer\": {\n                    \"type\": \"string\",\n                    \"description\": \"Organization that issued the certification.\"\n                  },\n                  \"dateObtained\": {\n\
  \                    \"type\": \"string\",\n                    \"description\": \"Date the certification was obtained.\"\n                  },\n                  \"expirationDate\": {\n                    \"type\": \"string\",\n                    \"description\": \"Expiration date of the certification, if applicable.\"\n                  }\n                }\n              }\n            },\n            \"summary\": {\n              \"type\": \"string\",\n              \"description\": \"Professional summary or objective from the resume.\"\n            }\n          }\n        }\n      }\n    },\n    \"coverLetter\": {\n      \"type\": \"string\",\n      \"description\": \"The candidate's cover letter text, if provided with the application.\"\n    },\n    \"applicationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The current disposition status of the candidate's application within the hiring pipeline. Must map to one of Indeed's six predefined categories.\",\n   \
  \   \"enum\": [\"NEW\", \"CONTACTED\", \"INTERVIEWED\", \"OFFERED\", \"HIRED\", \"REJECTED\"]\n    },\n    \"screenerQuestionResponses\": {\n      \"type\": \"array\",\n      \"description\": \"The candidate's responses to screener questions configured on the job posting.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"questionId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier of the screener question.\"\n          },\n          \"question\": {\n            \"type\": \"string\",\n            \"description\": \"The text of the screener question presented to the candidate.\"\n          },\n          \"answer\": {\n            \"type\": \"string\",\n            \"description\": \"The candidate's response to the screener question.\"\n          }\n        }\n      }\n    },\n    \"eeoResponses\": {\n      \"type\": \"object\",\n      \"description\": \"Equal Employment Opportunity (EEO) compliance responses\
  \ provided by the candidate. Only available for US employers that have EEO questions enabled on their job postings.\",\n      \"properties\": {\n        \"gender\": {\n          \"type\": \"string\",\n          \"description\": \"The candidate's self-reported gender identity.\"\n        },\n        \"race\": {\n          \"type\": \"string\",\n          \"description\": \"The candidate's self-reported race or ethnicity.\"\n        },\n        \"veteranStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The candidate's self-reported veteran status.\"\n        },\n        \"disabilityStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The candidate's self-reported disability status.\"\n        }\n      }\n    },\n    \"appliedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the candidate submitted their application.\"\n    },\n    \"source\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The channel through which the candidate submitted their application, such as indeed_apply, organic, or other integration sources.\"\n    },\n    \"jobPostingId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the job posting the candidate applied to.\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the job posting the candidate applied to.\"\n    },\n    \"employerId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the employer who posted the job.\"\n    },\n    \"acknowledged\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this candidate application has been acknowledged by the ATS. Unacknowledged applications are returned first in Retrieve Candidates API queries.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the candidate\
  \ record was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-candidate-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: Indeed Candidate
---
