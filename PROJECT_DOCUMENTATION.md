# Employee Raise Issue – Record Producer & Service Portal Integration

## Project Overview

The Employee Raise Issue project is a ServiceNow-based self-service solution that allows employees to raise workplace issues through a user-friendly Service Portal.

The project uses a custom scoped application, custom table, UI Policies, dependent fields, Record Producer, Service Portal, and custom widgets.

## Technologies Used

- ServiceNow
- ServiceNow Studio
- Custom Scoped Application
- Custom Tables
- UI Policies
- Dictionary Dependency
- Record Producer
- Service Portal
- Service Portal Widgets
- HTML
- CSS
- JavaScript / Client Script

## Project Phases

### Phase 1 – Creating a Custom Application

Created a custom scoped application named **Employee Center** using ServiceNow Studio.

### Phase 2 – Creating a Custom Table and Fields

Created the **Employee Raise Issue** custom table with fields:

- Number
- Requester
- Category
- Subcategory
- Short Description
- State
- Priority
- Assignment Group

### Phase 3 – Creating UI Policies and Dependency

Implemented UI Policies to control form behavior.

- Short Description becomes mandatory when State is New.
- Number field is read-only.
- Category and Subcategory are dependent fields.

Dependency:

- Network → VPN
- Hardware → Laptop
- Software → Server
- Access → Forgot password

### Phase 4 – Creating a Record Producer

Created a Record Producer named **Raise Employee Issue**.

The Record Producer allows employees to submit issues through the Service Portal. Variables are mapped to fields in the Employee Raise Issue table.

### Phase 5 – Creating a Service Portal

Created a dedicated Service Portal named **Requesting Portal** with the URL suffix:

`employee_request`

The portal provides employees with an easy interface to raise issues.

### Phase 6 – Creating Widgets

Created two custom Service Portal widgets:

1. Commercial Widget
2. Link Redirect / Raise Ticket Widget

HTML and CSS were used for the widget design.

A Client Script was used to redirect the user from the Raise Ticket widget to the Record Producer.

### Phase 7 – Testing and Validation

Performed end-to-end testing of:

- Service Portal
- Custom widgets
- Raise Employee Issue Record Producer
- Category/Subcategory dependency
- UI Policies
- Record creation in the backend table

### Phase 8 – Conclusion

The project provides a centralized and user-friendly solution for employees to raise workplace issues.

It improves issue submission, reduces manual effort, maintains structured data, and provides seamless integration between the Service Portal and backend ServiceNow records.

## Project Flow

Employee  
↓  
Service Portal  
↓  
Raise an Issue Widget  
↓  
Record Producer  
↓  
Employee Raise Issue Table  
↓  
Backend Record Created
