---
description: Controls the display frequency of the data returned. * **D** = Daily * **W** = Weekly, based on the last day of the week of the start date. * **M** = Monthly, based on the last trading day of the month. * **AM** = Monthly, based on the start date (e.g., if the start date is June 16, data is displayed for June 16, May 16, April 16 etc.). * **CQ** = Quarterly based on the last trading day of the calendar quarter (March, June, September, or December). * **FQ** = Fiscal Quarter of the company. * **AY** = Actual Annual, based on the start date. * **CY** = Calendar Annual, based on the last trading day of the calendar year. * **FY** = Fiscal Annual, based on the last trading day of the company's fiscal year.
layout: schema
name: frequency
properties_list: []
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-funds-frequency-schema.json
slug: factset-funds-frequency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"frequency\",\n  \"type\": \"string\",\n  \"description\": \"Controls the display frequency of the data returned.\\n  * **D** = Daily\\n  * **W** = Weekly, based on the last day of the week of the start date.\\n  * **M** = Monthly, based on the last trading day of the month.\\n  * **AM** = Monthly, based on the start date (e.g., if the start date is June 16, data is displayed for June 16, May 16, April 16 etc.).\\n  * **CQ** = Quarterly based on the last trading day of the calendar quarter (March, June, September, or December).\\n  * **FQ** = Fiscal Quarter of the company.\\n  * **AY** = Actual Annual, based on the start date.\\n  * **CY** = Calendar Annual, based on the last trading day of the calendar year.\\n  * **FY** = Fiscal Annual, based on the last trading day of the company's fiscal year.\\n\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-funds-frequency-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: frequency
---
