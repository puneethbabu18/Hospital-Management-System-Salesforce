visit My Salesforce trailhead Profile: https://www.salesforce.com/trailblazer/pggl9u4ca9ufowgo8m


🏥 Hospital Management System (Salesforce Project)

📌 Overview

This project is a Hospital Management System built on Salesforce. It helps manage patient records, schedule appointments, automate doctor assignment, and generate reports & dashboards for better decision-making.

---

🎯 Features

- Patient record management
- Appointment scheduling
- Automatic doctor assignment using Flow
- Email notification for appointment confirmation
- Reports and dashboards for analytics

---

🛠️ Technologies Used

- Salesforce Platform
- Apex (for backend logic)
- SOQL (for data retrieval)
- Flow Builder (automation)
- Reports & Dashboards

---

📂 Data Model

Objects Created:

- Patient
- Appointment

Relationships:

- One Patient → Many Appointments
- Appointment → Linked to Patient (Lookup Relationship)

---

⚙️ Implementation Steps

1. Patient Object

- Created custom object Patient
- Fields:
  - Age (Number)
  - Phone (Phone)

---

2. Appointment Object

- Created custom object Appointment
- Fields:
  - Appointment Date (Date)
  - Status (Picklist: Scheduled, Completed)
  - Patient (Lookup to Patient)
  - Department (Picklist: Cardiology, General)
  - Doctor Name (Text)
  - Description (Long Text)

---

3. Field Dependency

- Controlling Field: Department
- Dependent Field: Doctor Name
- Mapping:
  - Cardiology → Dr. A
  - General → Dr. B

---

4. Automation using Flow

- Record-Triggered Flow on Appointment
- Logic:
  - If Department = Cardiology → Assign Dr. A
  - If Department = General → Assign Dr. B

---

5. Email Notification

- Created Email Template:
  - “Your appointment is confirmed successfully”
- Integrated email action in Flow

---

6. Reports Created

- Appointments by Status
- Appointments by Department

---

7. Dashboard

- Pie Chart → Appointment Status
- Bar Chart → Department-wise appointments

---

🚀 Outcome

- Efficient patient and appointment management
- Automated doctor assignment
- Real-time reporting and visualization
- Improved operational efficiency

---

💡 Interview Explanation (Short)

Developed a Hospital Management System using Salesforce by creating custom objects, implementing field dependencies, automating processes with Flow, and building reports and dashboards for data insights.

---

📌 Future Enhancements

- Add Billing Module
- Integrate SMS Notifications
- Role-based access control
- Mobile app integration

---

👨‍💻 Author

Puneeth Babu
