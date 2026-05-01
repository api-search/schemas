---
description: <p>The domain to associate with an WorkMail organization.</p> <p>When you configure a domain hosted in Amazon Route 53 (Route 53), all recommended DNS records are added to the organization when you create it. For more information, see <a href="https://docs.aws.amazon.com/workmail/latest/adminguide/add_domain.html">Adding a domain</a> in the <i>WorkMail Administrator Guide</i>.</p>
layout: schema
name: Domain
properties_list:
- description: ''
  name: DomainName
  type: object
- description: ''
  name: HostedZoneId
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-domain-schema.json
slug: workmail-domain
source_filename: workmail-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The fully qualified domain name.\"\n        }\n      ]\n    },\n    \"HostedZoneId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HostedZoneId\"\n        },\n        {\n          \"description\": \"The hosted zone ID for a domain hosted in Route 53. Required when configuring a domain hosted in Route 53.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>The domain to associate with an WorkMail organization.</p> <p>When you configure a domain hosted in Amazon Route 53 (Route 53), all recommended DNS records are added to the organization when you create it. For more information, see <a href=\\\"https://docs.aws.amazon.com/workmail/latest/adminguide/add_domain.html\\\">Adding a domain</a> in the <i>WorkMail Administrator Guide</i>.</p>\"\
  ,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Domain\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-domain-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-domain-schema.json
tags:
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: Domain
---
