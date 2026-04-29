# Schema Assumptions

The following assumptions were made about the database structure:

## Patients Table
- id (Primary Key)
- name
- gender
- state

## Doctors Table
- id (Primary Key)
- name
- specialty

## Appointments Table
- id (Primary Key)
- patient_id (Foreign Key)
- doctor_id (Foreign Key)
- status (e.g., Confirmed, Pending)

## Relationships
- appointments.patient_id → patients.id
- appointments.doctor_id → doctors.id

## Notes
- State is derived from patients table
- Only confirmed appointments are considered in analysis
