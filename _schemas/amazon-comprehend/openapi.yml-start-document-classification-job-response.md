---
description: StartDocumentClassificationJobResponse schema
layout: schema
name: StartDocumentClassificationJobResponse
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobArn
  type: object
- description: ''
  name: JobStatus
  type: object
- description: ''
  name: DocumentClassifierArn
  type: object
provider_name: Amazon Comprehend
provider_slug: amazon-comprehend
schema_file: json-schema/openapi.yml-start-document-classification-job-response-schema.json
slug: openapi.yml-start-document-classification-job-response
source_filename: openapi.yml-start-document-classification-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-start-document-classification-job-response-schema.json\",\n  \"title\": \"StartDocumentClassificationJobResponse\",\n  \"description\": \"StartDocumentClassificationJobResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The identifier generated for the job. To get the status of the job, use this identifier with the <code>DescribeDocumentClassificationJob</code> operation.\"\n        }\n      ]\n    },\n    \"JobArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComprehendArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the document classification\
  \ job. It is a unique, fully qualified identifier for the job. It includes the Amazon Web Services account, Amazon Web Services Region, and the job ID. The format of the ARN is as follows:</p> <p> <code>arn:&lt;partition&gt;:comprehend:&lt;region&gt;:&lt;account-id&gt;:document-classification-job/&lt;job-id&gt;</code> </p> <p>The following is an example job ARN:</p> <p> <code>arn:aws:comprehend:us-west-2:111122223333:document-classification-job/1234abcd12ab34cd56ef1234567890ab</code> </p>\"\n        }\n      ]\n    },\n    \"JobStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the job:</p> <ul> <li> <p>SUBMITTED - The job has been received and queued for processing.</p> </li> <li> <p>IN_PROGRESS - Amazon Comprehend is processing the job.</p> </li> <li> <p>COMPLETED - The job was successfully completed and the output is available.</p> </li> <li> <p>FAILED - The job did\
  \ not complete. For details, use the <code>DescribeDocumentClassificationJob</code> operation.</p> </li> <li> <p>STOP_REQUESTED - Amazon Comprehend has received a stop request for the job and is processing the request.</p> </li> <li> <p>STOPPED - The job was successfully stopped without completing.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"DocumentClassifierArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentClassifierArn\"\n        },\n        {\n          \"description\": \"The ARN of the custom classification model.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-comprehend/refs/heads/main/json-schema/openapi.yml-start-document-classification-job-response-schema.json
tags:
- Machine Learning
- Natural Language Processing
- NLP
- Text Analysis
title: StartDocumentClassificationJobResponse
---
