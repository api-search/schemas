---
description: <p>A unique case-sensitive string used to ensure that this request is idempotent (executes only once).</p> <p>You should not reuse the same token for other requests. If you retry a request with the same client request token and the same parameters after the original request has completed successfully, the result of the original request is returned.</p> <important> <p>This token is listed as required, however, if you do not specify it, the Amazon Web Services SDKs automatically generate one for you. If you are not using the Amazon Web Services SDK or the CLI, you must provide this token or the request will fail.</p> </important>
layout: schema
name: ClientRequestToken
properties_list: []
provider_name: Amazon Well-Architected Tool
provider_slug: amazon-well-architected-tool
schema_file: json-schema/well-architected-tool-client-request-token-schema.json
slug: well-architected-tool-client-request-token
source_filename: well-architected-tool-client-request-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"description\": \"<p>A unique case-sensitive string used to ensure that this request is idempotent (executes only once).</p> <p>You should not reuse the same token for other requests. If you retry a request with the same client request token and the same parameters after the original request has completed successfully, the result of the original request is returned.</p> <important> <p>This token is listed as required, however, if you do not specify it, the Amazon Web Services SDKs automatically generate one for you. If you are not using the Amazon Web Services SDK or the CLI, you must provide this token or the request will fail.</p> </important>\",\n  \"minLength\": 1,\n  \"maxLength\": 2048,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClientRequestToken\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-client-request-token-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-well-architected-tool/refs/heads/main/json-schema/well-architected-tool-client-request-token-schema.json
tags:
- Architecture
- AWS
- Best Practices
- Cloud Governance
- Well-Architected
- Workloads
title: ClientRequestToken
---
