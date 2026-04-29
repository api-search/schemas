---
description: Schema representing an employee record in Oracle E-Business Suite Human Resources Management System (HRMS). Maps to PER_ALL_PEOPLE_F, PER_ALL_ASSIGNMENTS_F, PER_ADDRESSES, and PER_PHONES tables. Uses date-track versioning where records have effective start and end dates.
layout: schema
name: Oracle EBS Employee
properties_list:
- description: Unique person identifier (PER_ALL_PEOPLE_F.PERSON_ID)
  name: personId
  type: integer
- description: Employee number (PER_ALL_PEOPLE_F.EMPLOYEE_NUMBER)
  name: employeeNumber
  type: string
- description: Person type identifier (PER_PERSON_TYPES.PERSON_TYPE_ID)
  name: personTypeId
  type: integer
- description: Title (Mr., Mrs., Ms., Dr., etc.)
  name: title
  type:
  - string
  - 'null'
- description: First name
  name: firstName
  type: string
- description: Middle name(s)
  name: middleNames
  type:
  - string
  - 'null'
- description: Last name
  name: lastName
  type: string
- description: Name suffix (Jr., Sr., III, etc.)
  name: suffix
  type:
  - string
  - 'null'
- description: 'Full name (system-derived: LastName, Title FirstName MiddleNames Suffix)'
  name: fullName
  type: string
- description: Preferred/known-as name
  name: knownAs
  type:
  - string
  - 'null'
- description: Previous last name (maiden name)
  name: previousLastName
  type:
  - string
  - 'null'
- description: Email address
  name: emailAddress
  type:
  - string
  - 'null'
- description: Gender
  name: sex
  type: string
- description: Date of birth
  name: dateOfBirth
  type:
  - string
  - 'null'
- description: National identifier (Social Security Number, National Insurance Number, etc.)
  name: nationalIdentifier
  type:
  - string
  - 'null'
- description: Nationality lookup code
  name: nationality
  type:
  - string
  - 'null'
- description: Marital status lookup code
  name: maritalStatus
  type:
  - string
  - 'null'
- description: Registered disabled status
  name: registeredDisabledFlag
  type:
  - string
  - 'null'
- description: Date-track effective start date
  name: effectiveStartDate
  type: string
- description: Date-track effective end date (31-DEC-4712 for current records)
  name: effectiveEndDate
  type: string
- description: Original hire date (PER_PERIODS_OF_SERVICE.DATE_START)
  name: hireDate
  type: string
- description: Original date of hire (may differ from hire date for rehires)
  name: originalDateOfHire
  type:
  - string
  - 'null'
- description: Adjusted service date
  name: adjustedServiceDate
  type:
  - string
  - 'null'
- description: Actual termination date
  name: terminationDate
  type:
  - string
  - 'null'
- description: Whether the person is currently an active employee
  name: currentEmployeeFlag
  type: string
- description: Business group identifier (HR_ALL_ORGANIZATION_UNITS.ORGANIZATION_ID)
  name: businessGroupId
  type: integer
- description: Primary employee assignment
  name: assignment
  type: object
- description: All employee assignments (including secondary)
  name: assignments
  type: array
- description: Employee addresses
  name: addresses
  type: array
- description: Employee phone numbers
  name: phones
  type: array
- description: Current period of service
  name: periodOfService
  type: object
- description: User who created the record
  name: createdBy
  type: integer
- description: Record creation date
  name: creationDate
  type: string
- description: User who last updated the record
  name: lastUpdatedBy
  type: integer
- description: Record last update date
  name: lastUpdateDate
  type: string
- description: Object version number for optimistic locking
  name: objectVersionNumber
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/employee.json
slug: employee
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.oracle.com/ebs/employee.json\",\n  \"title\": \"Oracle EBS Employee\",\n  \"description\": \"Schema representing an employee record in Oracle E-Business Suite Human Resources Management System (HRMS). Maps to PER_ALL_PEOPLE_F, PER_ALL_ASSIGNMENTS_F, PER_ADDRESSES, and PER_PHONES tables. Uses date-track versioning where records have effective start and end dates.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"personId\",\n    \"lastName\",\n    \"effectiveStartDate\",\n    \"effectiveEndDate\"\n  ],\n  \"properties\": {\n    \"personId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique person identifier (PER_ALL_PEOPLE_F.PERSON_ID)\"\n    },\n    \"employeeNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Employee number (PER_ALL_PEOPLE_F.EMPLOYEE_NUMBER)\",\n      \"maxLength\": 30\n    },\n    \"personTypeId\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Person type identifier (PER_PERSON_TYPES.PERSON_TYPE_ID)\"\n    },\n    \"title\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Title (Mr., Mrs., Ms., Dr., etc.)\",\n      \"maxLength\": 30\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name\",\n      \"maxLength\": 150\n    },\n    \"middleNames\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Middle name(s)\",\n      \"maxLength\": 60\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name\",\n      \"maxLength\": 150\n    },\n    \"suffix\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Name suffix (Jr., Sr., III, etc.)\",\n      \"maxLength\": 30\n    },\n    \"fullName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name (system-derived: LastName, Title FirstName MiddleNames Suffix)\",\n      \"maxLength\": 240\n    },\n    \"knownAs\":\
  \ {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Preferred/known-as name\",\n      \"maxLength\": 80\n    },\n    \"previousLastName\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Previous last name (maiden name)\",\n      \"maxLength\": 150\n    },\n    \"emailAddress\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"Email address\",\n      \"maxLength\": 240\n    },\n    \"sex\": {\n      \"type\": \"string\",\n      \"description\": \"Gender\",\n      \"enum\": [\n        \"M\",\n        \"F\"\n      ]\n    },\n    \"dateOfBirth\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date of birth\"\n    },\n    \"nationalIdentifier\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"National identifier (Social Security Number, National Insurance Number, etc.)\",\n      \"maxLength\": 30\n    },\n    \"nationality\": {\n\
  \      \"type\": [\"string\", \"null\"],\n      \"description\": \"Nationality lookup code\"\n    },\n    \"maritalStatus\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Marital status lookup code\",\n      \"enum\": [\n        \"S\",\n        \"M\",\n        \"D\",\n        \"W\",\n        \"DP\",\n        \"L\",\n        null\n      ]\n    },\n    \"registeredDisabledFlag\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Registered disabled status\"\n    },\n    \"effectiveStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date-track effective start date\"\n    },\n    \"effectiveEndDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date-track effective end date (31-DEC-4712 for current records)\"\n    },\n    \"hireDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Original hire date (PER_PERIODS_OF_SERVICE.DATE_START)\"\
  \n    },\n    \"originalDateOfHire\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Original date of hire (may differ from hire date for rehires)\"\n    },\n    \"adjustedServiceDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Adjusted service date\"\n    },\n    \"terminationDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Actual termination date\"\n    },\n    \"currentEmployeeFlag\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the person is currently an active employee\",\n      \"enum\": [\n        \"Y\",\n        \"N\"\n      ]\n    },\n    \"businessGroupId\": {\n      \"type\": \"integer\",\n      \"description\": \"Business group identifier (HR_ALL_ORGANIZATION_UNITS.ORGANIZATION_ID)\"\n    },\n    \"assignment\": {\n      \"$ref\": \"#/$defs/Assignment\",\n      \"description\": \"Primary employee\
  \ assignment\"\n    },\n    \"assignments\": {\n      \"type\": \"array\",\n      \"description\": \"All employee assignments (including secondary)\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Assignment\"\n      }\n    },\n    \"addresses\": {\n      \"type\": \"array\",\n      \"description\": \"Employee addresses\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Address\"\n      }\n    },\n    \"phones\": {\n      \"type\": \"array\",\n      \"description\": \"Employee phone numbers\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Phone\"\n      }\n    },\n    \"periodOfService\": {\n      \"$ref\": \"#/$defs/PeriodOfService\",\n      \"description\": \"Current period of service\"\n    },\n    \"createdBy\": {\n      \"type\": \"integer\",\n      \"description\": \"User who created the record\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation date\"\n    },\n    \"lastUpdatedBy\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"User who last updated the record\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last update date\"\n    },\n    \"objectVersionNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Object version number for optimistic locking\"\n    }\n  },\n  \"$defs\": {\n    \"Assignment\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"assignmentId\"\n      ],\n      \"properties\": {\n        \"assignmentId\": {\n          \"type\": \"integer\",\n          \"description\": \"Assignment identifier (PER_ALL_ASSIGNMENTS_F.ASSIGNMENT_ID)\"\n        },\n        \"assignmentNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Assignment number\",\n          \"maxLength\": 30\n        },\n        \"assignmentType\": {\n          \"type\": \"string\",\n          \"description\": \"Assignment type: E=Employee, C=Contingent\
  \ Worker, A=Applicant\",\n          \"enum\": [\n            \"E\",\n            \"C\",\n            \"A\"\n          ]\n        },\n        \"primaryFlag\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this is the primary assignment\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"assignmentStatusTypeId\": {\n          \"type\": \"integer\",\n          \"description\": \"Assignment status type identifier\"\n        },\n        \"assignmentStatusName\": {\n          \"type\": \"string\",\n          \"description\": \"Assignment status (Active Assignment, Suspend Assignment, etc.)\"\n        },\n        \"jobId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Job identifier (PER_JOBS.JOB_ID)\"\n        },\n        \"jobName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Job name\"\n        },\n        \"positionId\": {\n          \"type\": [\"\
  integer\", \"null\"],\n          \"description\": \"Position identifier (HR_ALL_POSITIONS_F.POSITION_ID)\"\n        },\n        \"positionName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Position name\"\n        },\n        \"gradeId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Grade identifier (PER_GRADES.GRADE_ID)\"\n        },\n        \"gradeName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Grade name\"\n        },\n        \"organizationId\": {\n          \"type\": \"integer\",\n          \"description\": \"HR organization identifier\"\n        },\n        \"organizationName\": {\n          \"type\": \"string\",\n          \"description\": \"HR organization name\"\n        },\n        \"locationId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Work location identifier (HR_LOCATIONS_ALL.LOCATION_ID)\"\n        },\n        \"locationCode\": {\n\
  \          \"type\": [\"string\", \"null\"],\n          \"description\": \"Work location code\"\n        },\n        \"supervisorId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Supervisor person identifier\"\n        },\n        \"payrollId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"Payroll identifier (PAY_ALL_PAYROLLS_F.PAYROLL_ID)\"\n        },\n        \"peopleGroupId\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"People group identifier\"\n        },\n        \"employmentCategory\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Employment category: FR=Full-Time Regular, FT=Full-Time Temp, PR=Part-Time Regular, PT=Part-Time Temp\",\n          \"enum\": [\n            \"FR\",\n            \"FT\",\n            \"PR\",\n            \"PT\",\n            null\n          ]\n        },\n        \"normalHours\": {\n          \"type\": [\"number\", \"null\"\
  ],\n          \"description\": \"Normal working hours per period\"\n        },\n        \"frequency\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Working hours frequency: D=Day, W=Week, M=Month, Y=Year\",\n          \"enum\": [\n            \"D\",\n            \"W\",\n            \"M\",\n            \"Y\",\n            null\n          ]\n        },\n        \"salary\": {\n          \"type\": [\"number\", \"null\"],\n          \"description\": \"Salary amount (from PER_PAY_PROPOSALS)\"\n        },\n        \"salaryBasis\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Salary basis (Annual, Monthly, Hourly)\"\n        },\n        \"effectiveStartDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"effectiveEndDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"objectVersionNumber\": {\n          \"type\": \"integer\"\n        }\n    \
  \  }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"addressId\"\n      ],\n      \"properties\": {\n        \"addressId\": {\n          \"type\": \"integer\",\n          \"description\": \"Address identifier (PER_ADDRESSES.ADDRESS_ID)\"\n        },\n        \"addressType\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Address type lookup code\"\n        },\n        \"primaryFlag\": {\n          \"type\": \"string\",\n          \"description\": \"Whether this is the primary address\",\n          \"enum\": [\n            \"Y\",\n            \"N\"\n          ]\n        },\n        \"addressLine1\": {\n          \"type\": \"string\",\n          \"description\": \"Address line 1\",\n          \"maxLength\": 240\n        },\n        \"addressLine2\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Address line 2\",\n          \"maxLength\": 240\n        },\n        \"addressLine3\": {\n \
  \         \"type\": [\"string\", \"null\"],\n          \"description\": \"Address line 3\",\n          \"maxLength\": 240\n        },\n        \"townOrCity\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"City/town\",\n          \"maxLength\": 30\n        },\n        \"region1\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"County/province\",\n          \"maxLength\": 120\n        },\n        \"region2\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"State\",\n          \"maxLength\": 120\n        },\n        \"postalCode\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Postal/ZIP code\",\n          \"maxLength\": 30\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"description\": \"Country code (ISO 3166-1 alpha-2)\",\n          \"maxLength\": 60\n        },\n        \"telephoneNumber1\": {\n          \"type\": [\"string\", \"null\"\
  ],\n          \"description\": \"Primary phone at this address\"\n        },\n        \"telephoneNumber2\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Secondary phone at this address\"\n        },\n        \"dateFrom\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Address start date\"\n        },\n        \"dateTo\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Address end date\"\n        }\n      }\n    },\n    \"Phone\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"phoneId\"\n      ],\n      \"properties\": {\n        \"phoneId\": {\n          \"type\": \"integer\",\n          \"description\": \"Phone identifier (PER_PHONES.PHONE_ID)\"\n        },\n        \"phoneType\": {\n          \"type\": \"string\",\n          \"description\": \"Phone type: W1=Work, H1=Home, M=Mobile, WF=Work Fax, HF=Home Fax\",\n          \"\
  enum\": [\n            \"W1\",\n            \"H1\",\n            \"M\",\n            \"WF\",\n            \"HF\"\n          ]\n        },\n        \"phoneNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Phone number\",\n          \"maxLength\": 60\n        },\n        \"dateFrom\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"dateTo\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\"\n        }\n      }\n    },\n    \"PeriodOfService\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"periodOfServiceId\": {\n          \"type\": \"integer\",\n          \"description\": \"Period of service identifier (PER_PERIODS_OF_SERVICE.PERIOD_OF_SERVICE_ID)\"\n        },\n        \"dateStart\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Period start date (hire date)\"\n        },\n        \"actualTerminationDate\": {\n         \
  \ \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Actual termination date\"\n        },\n        \"finalProcessDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Final payroll process date\"\n        },\n        \"lastStandardProcessDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Last standard payroll process date\"\n        },\n        \"leavingReason\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Termination reason lookup code\"\n        },\n        \"notifiedTerminationDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\": \"Date termination was notified\"\n        },\n        \"adjustedServiceDate\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date\",\n          \"description\":\
  \ \"Adjusted service date\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/employee.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Oracle EBS Employee
---
