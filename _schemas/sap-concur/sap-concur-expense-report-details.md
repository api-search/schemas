---
description: The full representation of an expense report
layout: schema
name: ReportDetails
properties_list:
- description: Unique identifier of the expense report
  name: reportId
  type: string
- description: The name or title of the report
  name: name
  type: string
- description: The business justification for the expenses
  name: businessPurpose
  type: string
- description: The date of the report
  name: reportDate
  type: string
- description: The start date of the reporting period
  name: startDate
  type: string
- description: The end date of the reporting period
  name: endDate
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: countryCode
  type: string
- description: ISO 3166-2 subdivision code
  name: countrySubDivisionCode
  type: string
- description: ISO 4217 three-letter currency code
  name: currencyCode
  type: string
- description: The expense policy applied to this report
  name: policyId
  type: string
- description: The form template used for this report
  name: reportFormId
  type: string
- description: The financial ledger associated with this report
  name: ledgerId
  type: string
- description: Human-readable approval status label
  name: approvalStatus
  type: string
- description: Machine-readable approval status code
  name: approvalStatusId
  type: string
- description: Human-readable payment status label
  name: paymentStatus
  type: string
- description: Machine-readable payment status code
  name: paymentStatusId
  type: string
- description: The unique identifier of the report owner
  name: userId
  type: string
- description: Whether the report has been submitted
  name: isSubmitted
  type: boolean
- description: Whether the report was sent back for corrections
  name: isSentBack
  type: boolean
- description: When the report was created (ISO 8601)
  name: creationDate
  type: string
- description: When the report was last submitted (ISO 8601)
  name: submitDate
  type: string
- description: The version number, incremented on each modification
  name: reportVersion
  type: integer
- description: Custom field values on the report header
  name: customData
  type: array
- description: HATEOAS navigation links
  name: links
  type: array
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-report-details-schema.json
slug: sap-concur-expense-report-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportDetails\",\n  \"type\": \"object\",\n  \"description\": \"The full representation of an expense report\",\n  \"properties\": {\n    \"reportId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the expense report\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name or title of the report\"\n    },\n    \"businessPurpose\": {\n      \"type\": \"string\",\n      \"description\": \"The business justification for the expenses\"\n    },\n    \"reportDate\": {\n      \"type\": \"string\",\n      \"description\": \"The date of the report\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"The start date of the reporting period\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"description\": \"The end date of the reporting period\"\n    },\n    \"countryCode\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    },\n    \"countrySubDivisionCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-2 subdivision code\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 three-letter currency code\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"The expense policy applied to this report\"\n    },\n    \"reportFormId\": {\n      \"type\": \"string\",\n      \"description\": \"The form template used for this report\"\n    },\n    \"ledgerId\": {\n      \"type\": \"string\",\n      \"description\": \"The financial ledger associated with this report\"\n    },\n    \"approvalStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable approval status label\"\n    },\n    \"approvalStatusId\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable approval status code\"\n    },\n    \"paymentStatus\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Human-readable payment status label\"\n    },\n    \"paymentStatusId\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable payment status code\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the report owner\"\n    },\n    \"isSubmitted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the report has been submitted\"\n    },\n    \"isSentBack\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the report was sent back for corrections\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"description\": \"When the report was created (ISO 8601)\"\n    },\n    \"submitDate\": {\n      \"type\": \"string\",\n      \"description\": \"When the report was last submitted (ISO 8601)\"\n    },\n    \"reportVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"The version number, incremented\
  \ on each modification\"\n    },\n    \"customData\": {\n      \"type\": \"array\",\n      \"description\": \"Custom field values on the report header\"\n    },\n    \"links\": {\n      \"type\": \"array\",\n      \"description\": \"HATEOAS navigation links\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-report-details-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: ReportDetails
---
