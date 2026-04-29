---
description: ''
layout: schema
name: consensusEstimate
properties_list:
- description: Identifier that was used for the request.
  name: requestId
  type: string
- description: Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equit
  name: fsymId
  type: string
- description: 'Company''s Financial statement ''metric'' that is estimated. Use the factset-estimates/v#/metrics endpoint for a complete list. For more details, visit [Online Assistant Page #15034](https://oa.apps.fact'
  name: metric
  type: string
- description: The reporting interval for the estimate. This is derived from Estimate Date and is translated to the Period List = ANN, QTR, SEMI, LTMA, or NMTA.
  name: periodicity
  type: string
- description: 'Company''s ''fiscal period'' for the estimate record. Periods for periodicity of ANN = 1, and SEMI = 2. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598).'
  name: fiscalPeriod
  type: integer
- description: 'Company''s ''fiscal year'' for the estimate record. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)'
  name: fiscalYear
  type: integer
- description: 'Company''s ''fiscal end date'' for the estimate record expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)'
  name: fiscalEndDate
  type: string
- description: '''Fiscal period'' based on relationship to ''estimate date''. This is not applicable for fixed-consensus endpoint. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/'
  name: relativePeriod
  type: integer
- description: 'Date of estimate expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)'
  name: estimateDate
  type: string
- description: 'Currency code for adjusting the data. Use ''ESTIMATE'' as input value for the values in Estimate Currency. For a list of currency ISO codes, visit [Online Assistant Page #1470](https://oa.apps.factset.c'
  name: currency
  type: string
- description: Estimate currency of the requested Security
  name: estimateCurrency
  type: string
- description: 'Mean of estimates in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)'
  name: mean
  type: number
- description: 'Median of estimates in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)'
  name: median
  type: number
- description: 'Standard deviation of estimates in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)'
  name: standardDeviation
  type: number
- description: 'Highest estimate in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114).'
  name: high
  type: number
- description: 'Lowest estimate in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)'
  name: low
  type: number
- description: 'Count or NEST of estimates in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)'
  name: estimateCount
  type: integer
- description: 'Number of Up Revisions within the consensus for the metric and period. The default window size is 100 days For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/1611'
  name: up
  type: integer
- description: 'Number of Up Revisions within the consensus for the metric and period. The default window size is 100 days. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/161'
  name: down
  type: integer
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-estimates-consensus-estimate-schema.json
slug: factset-estimates-consensus-estimate
source_filename: factset-estimates-consensus-estimate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"consensusEstimate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier that was used for the request.\"\n    },\n    \"fsymId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Regional Security Identifier. Six alpha-numeric characters, excluding vowels, with an -R suffix (XXXXXX-R). Identifies the security's best regional security data series per currency. For equities, all primary listings per region and currency are allocated a regional-level permanent identifier. The regional-level permanent identifier will be available once a SEDOL representing the region/currency has been allocated and the identifiers are on FactSet.\"\n    },\n    \"metric\": {\n      \"type\": \"string\",\n      \"description\": \"Company's Financial statement 'metric' that is estimated. Use the factset-estimates/v#/metrics\
  \ endpoint for a complete list. For more details, visit [Online Assistant Page #15034](https://oa.apps.factset.com/pages/15034)\"\n    },\n    \"periodicity\": {\n      \"type\": \"string\",\n      \"description\": \"The reporting interval for the estimate. This is derived from Estimate Date and is translated to the Period List = ANN, QTR, SEMI, LTMA, or NMTA.\"\n    },\n    \"fiscalPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"Company's 'fiscal period' for the estimate record. Periods for periodicity of ANN = 1, and SEMI = 2. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598).\"\n    },\n    \"fiscalYear\": {\n      \"type\": \"integer\",\n      \"description\": \"Company's 'fiscal year' for the estimate record. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)\"\n    },\n    \"fiscalEndDate\": {\n      \"type\": \"string\",\n      \"description\": \"Company's 'fiscal end date'\
  \ for the estimate record expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)\"\n    },\n    \"relativePeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"'Fiscal period' based on relationship to 'estimate date'. This is not applicable for fixed-consensus endpoint. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)\"\n    },\n    \"estimateDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date of estimate expressed in YYYY-MM-DD format. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16598)\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code for adjusting the data. Use 'ESTIMATE' as input value for the values in Estimate Currency. For a list of currency ISO codes, visit [Online Assistant Page #1470](https://oa.apps.factset.com/pages/1470).\"\n    },\n\
  \    \"estimateCurrency\": {\n      \"type\": \"string\",\n      \"description\": \"Estimate currency of the requested Security\"\n    },\n    \"mean\": {\n      \"type\": \"number\",\n      \"description\": \"Mean of estimates in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)\"\n    },\n    \"median\": {\n      \"type\": \"number\",\n      \"description\": \"Median of estimates in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)\"\n    },\n    \"standardDeviation\": {\n      \"type\": \"number\",\n      \"description\": \"Standard deviation of estimates in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)\"\n    },\n    \"high\": {\n      \"type\": \"number\",\n      \"description\": \"Highest estimate in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114).\"\
  \n    },\n    \"low\": {\n      \"type\": \"number\",\n      \"description\": \"Lowest estimate in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)\"\n    },\n    \"estimateCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Count or NEST of estimates in consensus calculation. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114)\"\n    },\n    \"up\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of Up Revisions within the consensus for the metric and period. The default window size is 100 days For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114).\"\n    },\n    \"down\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of Up Revisions within the consensus for the metric and period. The default window size is 100 days. For more details, visit [Online Assistant Page #16598](https://oa.apps.factset.com/pages/16114).\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-estimates-consensus-estimate-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: consensusEstimate
---
