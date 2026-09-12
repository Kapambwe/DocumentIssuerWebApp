# Zambian Regulatory Bodies Sample Data

This directory contains sample data for various Zambian government regulatory bodies and agencies. Each subdirectory represents a specific regulator with JSON files containing 20 sample records.

## Regulatory Bodies

### 1. Bank of Zambia (BOZ)
**Directory:** `bank-of-zambia/`
**File:** `financial-licenses.json`
**Description:** Central bank of Zambia - regulates financial institutions
**Sample Data Types:**
- Commercial Banking Licenses
- Microfinance Institution Licenses
- Bureau de Change Licenses
- Insurance Licenses
- Pension Fund Licenses
- Mobile Money Licenses
- Securities Broker-Dealer Licenses
- Payment Service Provider Licenses
- And more financial service licenses

### 2. Patents and Companies Registration Agency (PACRA)
**Directory:** `pacra/`
**File:** `business-registrations.json`
**Description:** Regulates business registration, intellectual property, and company law
**Sample Data Types:**
- Company Incorporation Certificates
- Business Trading Licenses
- Patent Certificates
- Trademark Registrations
- NGO Registrations
- Partnership Agreements
- Industrial Design Certificates
- Copyright Certificates
- Company Name Changes
- Share Certificates

### 3. Health Professions Council of Zambia (HPCZ)
**Directory:** `hpcz/`
**File:** `professional-licenses.json`
**Description:** Regulates health professionals
**Sample Data Types:**
- Medical Doctors
- Nurses (various specializations)
- Pharmacists
- Dentists
- Clinical Officers
- Radiographers
- Environmental Health Officers
- Physiotherapists

### 4. Zambia Institute of Chartered Accountants (ZICA)
**Directory:** `zica/`
**File:** `professional-licenses.json`
**Description:** Regulates accounting and auditing professionals
**Sample Data Types:**
- Chartered Accountants
- Certified Accountants
- Specializations: Auditing, Tax, Financial Management, Forensic Accounting

### 5. Law Association of Zambia (LAZ)
**Directory:** `laz/`
**File:** `professional-licenses.json`
**Description:** Regulates legal practitioners
**Sample Data Types:**
- Advocates
- Legal Practitioners
- Specializations: Criminal Law, Corporate Law, Family Law, Constitutional Law

### 6. Engineering Institution of Zambia (EIZ)
**Directory:** `eiz/`
**File:** `professional-licenses.json`
**Description:** Regulates engineering professionals
**Sample Data Types:**
- Professional Engineers
- Engineering Technologists
- Engineering Technicians
- Specializations: Civil, Electrical, Mechanical, Mining Engineering

### 7. Teaching Council of Zambia (TCZ)
**Directory:** `tcz/`
**File:** `professional-licenses.json`
**Description:** Regulates teaching professionals
**Sample Data Types:**
- Registered Teachers
- Lecturer Teachers
- Specializations: Mathematics, Science, English Language, Social Studies

### 8. Road Transport and Safety Agency (RTSA)
**Directory:** `rtsa/`
**File:** `driver-licenses.json`
**Description:** Issues driver's licenses and regulates road transport
**Sample Data Types:**
- Driver's Licenses (Classes A, B, C, D)
- Digital Driver's Licenses (mDL)
- License points tracking
- Traffic violation records

### 9. Examinations Council of Zambia (ECZ)
**Directory:** `ecz/`
**File:** `examination-certificates.json`
**Description:** Sets and administers national examinations and issues certificates
**Sample Data Types:**
- Grade 12 Certificates (GCE - General Certificate of Education)
- Grade 9 Certificates (JSC - Junior Secondary Certificate)
- Grade 7 Certificates (PSLC - Primary School Leaving Certificate)
- Certificate of Equivalence (foreign certificate recognition)
- Certificate Verification Documents

## Data Structure

All JSON files contain arrays of 20 items. Each item represents a document or license issued by the respective regulatory body.

### Common Fields
Most documents include:
- `DocumentId` - Unique identifier
- `DocumentNumber` - Official document/license number
- `DocumentType` - Type of document
- `IssuerName` - Name of the issuing authority
- `CitizenNRC` - National Registration Card number
- `CitizenName` / `FullName` - Name of the holder
- `IssueDate` - Date of issuance
- `Status` - Current status (Active, Expired, etc.)
- `IsSigned` - Whether digitally signed

### Professional License Additional Fields
Professional licenses (HPCZ, ZICA, LAZ, EIZ, TCZ) also include:
- `ProfessionType` - Type of profession
- `ProfessionSpecialization` - Area of specialization
- `RegulatoryBody` - Full name of the regulatory authority
- `CPDPointsRequired/Earned` - Continuing Professional Development tracking
- `HasCurrentPracticingCertificate` - Annual practicing certificate status
- `IsInGoodStanding` - Good standing verification

## Usage

These JSON files can be used to:
1. Populate mock services for testing
2. Demonstrate government document issuance workflows
3. Test multi-agency document verification systems
4. Showcase digital credential and OpenID4VC implementations

## Notes

- All data is fictional and created for demonstration purposes
- NRC numbers follow Zambian format: ######/##/#
- Phone numbers use Zambian format: +260 9X XXXXXXX
- All dates are in ISO 8601 format
- Each regulator has exactly 20 sample records

## Last Updated
February 2026
