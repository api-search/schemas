---
description: A payslip represents a worker's pay statement for a specific pay period, detailing earnings, deductions, taxes, and net pay amounts along with year-to-date totals.
layout: schema
name: Workday Payroll Payslip
properties_list:
- description: Unique identifier for the payslip
  name: id
  type: string
- description: ''
  name: worker
  type: object
- description: ''
  name: payPeriod
  type: object
- description: Date of payment
  name: paymentDate
  type: string
- description: Total gross pay for the period
  name: grossPay
  type: number
- description: Total net pay after all deductions and taxes
  name: netPay
  type: number
- description: Sum of all earnings for the period
  name: totalEarnings
  type: number
- description: Sum of all deductions for the period
  name: totalDeductions
  type: number
- description: Sum of all tax withholdings for the period
  name: totalTaxes
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Itemized earnings breakdown
  name: earnings
  type: array
- description: Itemized deductions breakdown
  name: deductions
  type: array
- description: Itemized tax withholdings breakdown
  name: taxes
  type: array
- description: Year-to-date gross pay
  name: yearToDateGross
  type: number
- description: Year-to-date net pay
  name: yearToDateNet
  type: number
- description: Year-to-date tax withholdings
  name: yearToDateTaxes
  type: number
provider_name: Workday Payroll
provider_slug: workday-payroll
schema_file: json-schema/workday-payroll-payslip-schema.json
slug: workday-payroll-payslip
source_filename: workday-payroll-payslip-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://community.workday.com/schemas/workday-payroll/payslip.json\",\n  \"title\": \"Workday Payroll Payslip\",\n  \"description\": \"A payslip represents a worker's pay statement for a specific pay period, detailing earnings, deductions, taxes, and net pay amounts along with year-to-date totals.\",\n  \"type\": \"object\",\n  \"required\": [\"worker\", \"payPeriod\", \"grossPay\", \"netPay\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the payslip\"\n    },\n    \"worker\": {\n      \"$ref\": \"#/$defs/WorkerRef\"\n    },\n    \"payPeriod\": {\n      \"$ref\": \"#/$defs/PayPeriod\"\n    },\n    \"paymentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of payment\"\n    },\n    \"grossPay\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total\
  \ gross pay for the period\"\n    },\n    \"netPay\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total net pay after all deductions and taxes\"\n    },\n    \"totalEarnings\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Sum of all earnings for the period\"\n    },\n    \"totalDeductions\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Sum of all deductions for the period\"\n    },\n    \"totalTaxes\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Sum of all tax withholdings for the period\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"earnings\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/EarningLine\"\n      },\n      \"description\": \"Itemized earnings breakdown\"\n    },\n    \"deductions\": {\n\
  \      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DeductionLine\"\n      },\n      \"description\": \"Itemized deductions breakdown\"\n    },\n    \"taxes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TaxLine\"\n      },\n      \"description\": \"Itemized tax withholdings breakdown\"\n    },\n    \"yearToDateGross\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Year-to-date gross pay\"\n    },\n    \"yearToDateNet\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Year-to-date net pay\"\n    },\n    \"yearToDateTaxes\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Year-to-date tax withholdings\"\n    }\n  },\n  \"$defs\": {\n    \"WorkerRef\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a worker in the Workday system\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"Worker unique identifier\"\n        },\n        \"descriptor\": {\n          \"type\": \"string\",\n          \"description\": \"Worker display name\"\n        }\n      }\n    },\n    \"PayPeriod\": {\n      \"type\": \"object\",\n      \"description\": \"Date range defining the pay period\",\n      \"required\": [\"startDate\", \"endDate\"],\n      \"properties\": {\n        \"startDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Start date of the pay period\"\n        },\n        \"endDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"End date of the pay period\"\n        }\n      }\n    },\n    \"EarningLine\": {\n      \"type\": \"object\",\n      \"description\": \"A single line item for an earning on the payslip\",\n      \"properties\": {\n        \"earningCode\": {\n          \"type\": \"string\",\n          \"description\": \"Earning code\
  \ descriptor\"\n        },\n        \"currentAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Current period amount\"\n        },\n        \"currentHours\": {\n          \"type\": \"number\",\n          \"description\": \"Current period hours worked\"\n        },\n        \"rate\": {\n          \"type\": \"number\",\n          \"description\": \"Pay rate applied\"\n        },\n        \"yearToDateAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Year-to-date total for this earning\"\n        }\n      }\n    },\n    \"DeductionLine\": {\n      \"type\": \"object\",\n      \"description\": \"A single line item for a deduction on the payslip\",\n      \"properties\": {\n        \"deductionCode\": {\n          \"type\": \"string\",\n          \"description\": \"Deduction code descriptor\"\n        },\n        \"employeeAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Employee contribution amount\"\n        },\n  \
  \      \"employerAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Employer contribution amount\"\n        },\n        \"preTax\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the deduction is pre-tax\"\n        },\n        \"yearToDateEmployee\": {\n          \"type\": \"number\",\n          \"description\": \"Year-to-date employee amount\"\n        },\n        \"yearToDateEmployer\": {\n          \"type\": \"number\",\n          \"description\": \"Year-to-date employer amount\"\n        }\n      }\n    },\n    \"TaxLine\": {\n      \"type\": \"object\",\n      \"description\": \"A single line item for a tax withholding on the payslip\",\n      \"properties\": {\n        \"taxAuthority\": {\n          \"type\": \"string\",\n          \"description\": \"Tax authority name\"\n        },\n        \"taxType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of tax\"\n        },\n        \"currentAmount\": {\n    \
  \      \"type\": \"number\",\n          \"description\": \"Current period tax amount\"\n        },\n        \"yearToDateAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Year-to-date tax amount\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-payroll/refs/heads/main/json-schema/workday-payroll-payslip-schema.json
tags:
- Compensation
- Enterprise
- Human-Resources
- Payroll
- Saas
- Tax
title: Workday Payroll Payslip
---
