# GLPI IT Service Desk Lab

## Project Overview

This project demonstrates a simulated IT Service Desk environment using **GLPI**, deployed with **Docker Desktop**.

The goal was to gain hands-on experience with IT support workflows, including ticket management, user roles, approval processes, task management, and IT asset tracking.

The lab simulates common responsibilities of an **L1/L2 IT Support Technician**.

## Technologies Used

- GLPI (IT Service Management)
- Docker Desktop
- Docker Compose
- MySQL
- Windows 11
- PowerShell

## Lab Environment

GLPI was deployed locally using Docker Compose.

The environment includes:

- GLPI application container
- MySQL database container
- Persistent Docker volumes
- Web interface accessible through `http://localhost`

## User Roles

Different GLPI accounts were configured to simulate a corporate IT environment.

| Role | Responsibility |
|---|---|
| End User | Submits IT support requests |
| IT Technician | Processes tickets and manages IT assets |
| IT Manager | Reviews and approves requests |

## Scenario: Second Monitor Request

**Ticket:** #52

**Type:** Service Request

**Requester:** Adam Smith, Finance Department

**Workstation:** WIN11-CLIENT01

### 1. Ticket Creation

An employee submitted a request for a second monitor to improve productivity when working with multiple applications and Excel spreadsheets.

Requested equipment:

- 24-inch monitor
- Compatible HDMI or DisplayPort cable

### 2. Manager Approval

The IT Technician submitted an approval request to the IT Manager.

The manager reviewed and approved the equipment request using GLPI's approval workflow.

### 3. Technician Task

A technician task was created to:

- Check monitor availability in inventory.
- Verify workstation compatibility.
- Prepare the monitor for assignment.

### 4. IT Asset Management

A monitor was registered in GLPI's asset inventory.

| Property | Value |
|---|---|
| Asset Name | MON-001 |
| Asset Type | Monitor |
| Screen Size | 24 inches |
| Inventory Number | IT-2026-001 |
| Assigned User | Adam Smith |
| Workstation | WIN11-CLIENT01 |

The monitor was linked to the service request to maintain asset traceability.

### 5. Ticket Resolution

The simulated workflow concludes with the approved monitor assigned to the employee and the request documented for resolution.

This demonstrates how IT Service Desk teams can track equipment requests from submission to completion.

## Screenshots

### Ticket and Service Request

![Service Request](screenshots/01-ticket-created.png)

### Manager Approval Request

![Manager Approval](screenshots/02-manager-approval.png)

### Approval Granted

![Approved Request](screenshots/03-approval-granted.png)

### Technician Task

![Technician Task](screenshots/04-technician-task.png)

### Asset Management

![Monitor Asset](screenshots/05-asset-management.png)

### Ticket Resolution

![Ticket Resolution](screenshots/06-ticket-resolved.png)

## Skills Demonstrated

- IT Service Management (ITSM)
- Helpdesk ticket lifecycle management
- Incident vs. Service Request classification
- Role-based user management
- Approval workflows
- IT asset inventory and assignment
- Technical documentation
- Docker container deployment
- Basic IT support processes

## Key Takeaways

This lab provided practical experience with GLPI and helped me understand how IT support teams manage employee requests, coordinate approvals, assign equipment, and maintain documentation.

It also strengthened my understanding of structured IT Service Desk processes in a simulated business environment.

---

**Disclaimer:** This project was completed in a personal training lab. All users, devices, assets, and support scenarios are simulated.

## Screenshots

### User Accounts
![GLPI User Accounts](02-user-accounts.png)

### Technician Role
![Technician Permissions](03-technician-role.png)

### Manager Role
![Manager Permissions](04-manager-role.png)
