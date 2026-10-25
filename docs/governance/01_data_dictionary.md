# Data Dictionary

## Taxpayer

| Field | Data Type | Description | Source | Sensitivity |
|---------|---------|---------|---------|---------|
| TaxpayerID | Integer | Internal taxpayer identifier | Taxpayer Master | Internal |
| SSN | String | Social Security Number | Taxpayer Master | Restricted |
| FilingStatus | String | Filing classification | Tax Return | Confidential |

## W2

| Field | Data Type | Description | Source | Sensitivity |
|---------|---------|---------|---------|---------|
| W2ID | Integer | Unique W2 record | Employer Reporting | Internal |
| EmployerID | Integer | Employer identifier | Employer Registry | Internal |
| Wages | Decimal | Reported wage income | Employer Reporting | Confidential |

## 1099

## PIT_Return

## Payments

## Employers

## Cases