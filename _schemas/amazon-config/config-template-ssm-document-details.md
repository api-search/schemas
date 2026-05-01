---
description: <p>This API allows you to create a conformance pack template with an Amazon Web Services Systems Manager document (SSM document). To deploy a conformance pack using an SSM document, first create an SSM document with conformance pack content, and then provide the <code>DocumentName</code> in the <a href="https://docs.aws.amazon.com/config/latest/APIReference/API_PutConformancePack.html">PutConformancePack API</a>. You can also provide the <code>DocumentVersion</code>.</p> <p>The <code>TemplateSSMDocumentDetails</code> object contains the name of the SSM document and the version of the SSM document.</p>
layout: schema
name: TemplateSSMDocumentDetails
properties_list:
- description: ''
  name: DocumentName
  type: object
- description: ''
  name: DocumentVersion
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-template-ssm-document-details-schema.json
slug: config-template-ssm-document-details
source_filename: config-template-ssm-document-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-template-ssm-document-details-schema.json\",\n  \"title\": \"TemplateSSMDocumentDetails\",\n  \"description\": \"<p>This API allows you to create a conformance pack template with an Amazon Web Services Systems Manager document (SSM document). To deploy a conformance pack using an SSM document, first create an SSM document with conformance pack content, and then provide the <code>DocumentName</code> in the <a href=\\\"https://docs.aws.amazon.com/config/latest/APIReference/API_PutConformancePack.html\\\">PutConformancePack API</a>. You can also provide the <code>DocumentVersion</code>.</p> <p>The <code>TemplateSSMDocumentDetails</code> object contains the name of the SSM document and the version of the SSM document.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentName\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SSMDocumentName\"\n        },\n        {\n          \"description\": \"The name or Amazon Resource Name (ARN) of the SSM document to use to create a conformance pack. If you use the document name, Config checks only your account and Amazon Web Services Region for the SSM document. If you want to use an SSM document from another Region or account, you must provide the ARN.\"\n        }\n      ]\n    },\n    \"DocumentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SSMDocumentVersion\"\n        },\n        {\n          \"description\": \"<p>The version of the SSM document to use to create a conformance pack. By default, Config uses the latest version.</p> <note> <p>This field is optional.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DocumentName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-template-ssm-document-details-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: TemplateSSMDocumentDetails
---
