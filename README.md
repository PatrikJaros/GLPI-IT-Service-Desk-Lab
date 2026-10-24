# IT Helpdesk & Ticketing System Lab

**GLPI | Docker | MySQL | IT Support L1/L2**

## Project Overview

I built a working IT Helpdesk and Ticketing System using GLPI and Docker Desktop.

The goal was to practice how IT Support Technicians manage employee requests, investigate technical problems, assign tickets, approve equipment requests, and track IT assets.

The project includes two simulated support scenarios:

1. **Incident:** A user cannot log in to their Windows domain account.
2. **Service Request:** An employee requests a second monitor.

All scenarios were performed in a personal training environment.

## Technologies Used

- **GLPI:** Ticket management and IT asset tracking
- **Docker Desktop:** Container management
- **Docker Compose:** Application deployment
- **MySQL:** Database
- **Windows 11:** Host operating system
- **PowerShell:** Docker commands and environment setup

## 1. Lab Setup

GLPI was deployed locally using Docker Compose.

The environment contains:

- A GLPI application container
- A MySQL database container
- Persistent Docker volumes
- A web interface available at `http://localhost`

## 2. User Accounts and Permissions

I configured three user accounts to simulate a small company's IT support environment.

| Account | GLPI Role | Responsibility |
|---|---|---|
| Adam Smith | Self-Service | Submits IT support requests |
| Technician IT | Technician | Investigates and resolves tickets |
| Manager IT | Supervisor | Reviews and approves requests |

### User Accounts

![User Accounts](02-user-accounts.png)

### Technician Permissions

![Technician Permissions](03-technician-role.png)

### Manager Permissions

![Manager Permissions](04-manager-role.png)

### End User Permissions

![End User Permissions](05-end-user-role.png)

## 3. Incident Management: Windows Login Problem

**Ticket #1 | Incident | High Priority**

### The Problem

An employee reported that they could not log in to their Windows workstation.

The error indicated that the domain account was locked.

### Investigation

I simulated an L1 IT Support troubleshooting process:

1. Verified the user's identity.
2. Asked when the problem started.
3. Identified a recent password change.
4. Investigated multiple login attempts using the old password.
5. Documented the suspected account lockout.

### Investigation Screenshot

![Incident Investigation](06-incident-investigation.png)

### Resolution

I documented a simulated resolution involving:

1. Checking the account status in Active Directory.
2. Confirming the account lockout.
3. Unlocking the account.
4. Testing login with the updated password.
5. Confirming access to company resources.

**Root Cause:** Multiple failed login attempts using an outdated password.

**Final Status:** Closed

![Incident Resolution](07-incident-resolution
