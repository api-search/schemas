---
description: Specifies the Auto-Tune state for the Elasticsearch domain. For valid states see the <a href="https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html" target="_blank">Developer Guide</a>.
layout: schema
name: AutoTuneState
properties_list: []
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-auto-tune-state-schema.json
slug: openapi-auto-tune-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-state-schema.json\",\n  \"title\": \"AutoTuneState\",\n  \"description\": \"Specifies the Auto-Tune state for the Elasticsearch domain. For valid states see the <a href=\\\"https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/auto-tune.html\\\" target=\\\"_blank\\\">Developer Guide</a>.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ENABLED\",\n    \"DISABLED\",\n    \"ENABLE_IN_PROGRESS\",\n    \"DISABLE_IN_PROGRESS\",\n    \"DISABLED_AND_ROLLBACK_SCHEDULED\",\n    \"DISABLED_AND_ROLLBACK_IN_PROGRESS\",\n    \"DISABLED_AND_ROLLBACK_COMPLETE\",\n    \"DISABLED_AND_ROLLBACK_ERROR\",\n    \"ERROR\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-auto-tune-state-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AutoTuneState
---
