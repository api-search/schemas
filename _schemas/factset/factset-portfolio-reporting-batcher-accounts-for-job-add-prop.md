---
description: The details of the account under the task in the object key
layout: schema
name: accountsForJobAddProp
properties_list:
- description: Indicates whether or not the parent portfolio is included as a separate portfolio when isSplit is true
  name: includeParent
  type: boolean
- description: Indicates whether the portfolio's components if any would be treated as individual portfolios when the job is run
  name: isSplit
  type: boolean
- description: When selected, the ACTM/CSTM will be split and will only return components that are still held in the ACTM. I.e., when the end date is "Latest," it will not return components where the end date occurs
  name: latestComponentsOnly
  type: boolean
- description: The number of levels when isSplit is true that the job will expand down to for a composite portfolio (CSTM or ACTM). "1" means only the first level will be expanded. "all" will be the value if all lev
  name: level
  type: string
- description: The full file path including portfolio name and type
  name: portfolioId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-portfolio-reporting-batcher-accounts-for-job-add-prop-schema.json
slug: factset-portfolio-reporting-batcher-accounts-for-job-add-prop
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"accountsForJobAddProp\",\n  \"type\": \"object\",\n  \"description\": \"The details of the account under the task in the object key\",\n  \"properties\": {\n    \"includeParent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether or not the parent portfolio is included as a separate portfolio when isSplit is true\"\n    },\n    \"isSplit\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the portfolio's components if any would be treated as individual portfolios when the job is run\"\n    },\n    \"latestComponentsOnly\": {\n      \"type\": \"boolean\",\n      \"description\": \"When selected, the ACTM/CSTM will be split and will only return components that are still held in the ACTM. I.e., when the end date is \\\"Latest,\\\" it will not return components where the end date occurs before Latest.\"\n    },\n    \"level\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The number of levels when isSplit is true that the job will expand down to for a composite portfolio (CSTM or ACTM). \\\"1\\\" means only the first level will be expanded. \\\"all\\\" will be the value if all levels are expanded down.\"\n    },\n    \"portfolioId\": {\n      \"type\": \"string\",\n      \"description\": \"The full file path including portfolio name and type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-portfolio-reporting-batcher-accounts-for-job-add-prop-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: accountsForJobAddProp
---
