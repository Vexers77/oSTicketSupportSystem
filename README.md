# oSTicketSupportSystem
Using osTicket Support System for setting up a Help Desk lab environment and making Ticket Examples, This guide provides a step-by-step walkthrough for setting up and managing roles, departments, teams, and additional configurations in osTicket after initial installation. These steps ensure that your help desk is properly organized, enabling efficient support operations.

---

## Table of Contents
1. [Overview](#overview)
2. [Setting Up Roles](#setting-up-roles)
3. [Creating Departments](#creating-departments)
4. [Configuring Teams](#configuring-teams)
5. [Public Ticket Creation](#public-ticket-creation)
6. [Creating Agents](#creating-agents)
7. [Adding Users](#adding-users)
8. [Setting Up SLA Plans](#setting-up-sla-plans)
9. [Creating Help Topics](#creating-help-topics)

---

## Overview

After singing up for an osTicket Support Sytem account,  this guide will help you with essential system administration tasks and  setup. These steps include creating roles, departments, teams, agents, and user configurations, and setting up SLA plans and help topics to streamline your support workflow.

---

## 1. Setting Up Roles

Roles in osTicket determine agents' permissions and access levels. Follow these steps to create a new role:
- **Path**: `Admin Panel > Agents > Roles`
- Click on **Add New Role** and enter the role name.
- **Example**: Create a role called **Supreme Admin** with all permissions enabled.
- ![Screenshot 2024-11-02 055837](https://github.com/user-attachments/assets/d7519d27-c536-419f-b507-909b9ecdf614)
  
- ![Screenshot 2024-11-02 060004](https://github.com/user-attachments/assets/fcdd80ba-bc1c-4f27-920f-1dad9a68769f)
  
- ![Screenshot 2024-11-02 060013](https://github.com/user-attachments/assets/01d96e0b-e160-4e80-8e9f-b0275a32c778)



> **Note**: Roles define agents' permissions. Only specific agents should have full administrative access.

---

## 2. Creating Departments

Departments are designed to assign agents according to their roles within the help desk.
- **Path**: `Admin Panel > Agents > Departments`
- **Example**: Create a department named **System Administrators**. This will house the Supreme Admins and can have settings like SLAs, managers, and email configurations.
- ![Screenshot 2024-11-02 060406](https://github.com/user-attachments/assets/f6a704f5-29ff-42e6-a2d4-f0bd555d165a)
  
- ![Screenshot 2024-11-02 060518](https://github.com/user-attachments/assets/fe090482-9ff8-44ed-82f8-e487001f561a)



---

## 3. Configuring Teams

Teams allow you to group agents from different departments to work on specific issues.
- **Path**: `Admin Panel > Agents > Teams`
- **Example**: Create a **Level II Support Team** to handle advanced issues that may require cross-department collaboration.
- ![Screenshot 2024-11-02 060626](https://github.com/user-attachments/assets/392d78cd-773c-4b68-8774-6c5f53fdb458)
  
- ![Screenshot 2024-11-02 060636](https://github.com/user-attachments/assets/c3658c9c-b0a3-4264-8f45-91ab54e6c33d)



> **Tip**: Teams can be useful for creating specialized support groups for certain products or high-level customer inquiries.

---

## 4. Public Ticket Creation

To allow anyone to create tickets in your osTicket system:
- **Path**: `Admin Panel > Settings > User Settings`
- Enable public ticket creation to let users submit support requests without pre-authorization.
- ![Screenshot 2024-11-02 060830](https://github.com/user-attachments/assets/297d8cc7-58b5-435d-9eb2-fc2a565e0dcb)


---

## 5. Creating Agents

Agents are responsible for resolving tickets. Agents can be assigned primary departments and roles based on the department.
- **Path**: `Admin Panel > Agents > Add New Agent`
- Assign each agent to their department, define their role, and set permissions.
- ![Screenshot 2024-11-02 061324](https://github.com/user-attachments/assets/7b7a9bcf-5411-4b59-8856-52b954e3303f)





> **Note**: Agents may have access to multiple departments but will have specific roles for each.

---

## 6. Adding Users

Users are the end customers who create tickets when they encounter issues.
- **Path**: `Agent Panel > Users > User Directory > Add New`
- Users are identified by their email addresses and can create and monitor their tickets through the system.
- ![Screenshot 2024-11-02 061503](https://github.com/user-attachments/assets/4986a475-f72c-41a1-97e8-ea2210f1260f)
  
- ![Screenshot 2024-11-02 062051](https://github.com/user-attachments/assets/9202e008-9367-44a5-b566-47ef0f7a8254)
  
- ![Screenshot 2024-11-02 062418](https://github.com/user-attachments/assets/54a4df2c-14ef-4fd5-9efa-e0640317ff03)


---

## 7. Setting Up SLA Plans

SLA (Service Level Agreement) Plans define response and resolution times for tickets.
- **Path**: `Admin Panel > Manage > SLA Plans`
- **Example**: Create an SLA plan for critical issues. For instance, **SEV-A** with a 24/7 schedule and a 1-hour grace period for high-priority incidents.
- ![Screenshot 2024-11-02 062651](https://github.com/user-attachments/assets/56a4c552-2312-425b-9b75-26425fd24ea0)
  
- ![Screenshot 2024-11-02 062703](https://github.com/user-attachments/assets/0de3cfd6-7b92-42d9-910b-2d8f00e2f84d)



---

## 8. Creating Help Topics

Help topics help users categorize their tickets, aiding in faster issue resolution.
- **Path**: `Admin Panel > Manage > Help Topics`
- **Example**: Set up a help topic like **Business Critical Outage** for significant issues such as mobile banking disruptions.
- ![Screenshot 2024-11-02 062821](https://github.com/user-attachments/assets/4fa0e564-7ea7-48c5-a1fe-5cf5b1e52e4c)

- ![Screenshot 2024-11-02 062837](https://github.com/user-attachments/assets/85e735eb-6114-4152-88fb-deb33b4f357f)



## 9. Ticket Lifecycle

This section describes the lifecycle of a ticket from creation by an end user through prioritization, assignment, and resolution.

### 9.1 Creating a Ticket as an End User

End users can create tickets when they experience issues. For example, in this case:

- **User**: Rebecca
- **Help Topic**: Business Critical Outage
- **Issue**: Customers cannot access mobile banking

- ![Screenshot 2024-11-02 063526](https://github.com/user-attachments/assets/33172753-0438-4b9a-873c-985a25cf1d25)



After submission, tickets are visible in the **Agent Panel** for agents and managers to review.

### 9.2 Ticket Monitoring and Assignment

Once a ticket is created, agents can monitor live tickets via the **Agent Panel**. Queue managers handle:

- **Ticket Assignment**: Assign tickets to the appropriate agents based on the issue.
- **SLA Application**: Apply relevant SLA plans to set response and resolution timelines.

- 
![Screenshot 2024-11-02 063545](https://github.com/user-attachments/assets/735e03af-395e-478f-b8c6-3ef7ffac7d0c)

> **Tip**: Queue managers ensure that high-priority tickets are routed promptly to appropriate agents, reducing response times for critical issues.

### 9.3 Setting Ticket Priority and SLA

For urgent issues, queue managers set the ticket priority and update the SLA plan to ensure a quick response. In this example:

- **Priority Level**: Emergency (due to high business impact)
- **SLA Plan**: Adjusted for rapid resolution, and a top-level technician is assigned to handle the case.

- ![Screenshot 2024-11-02 063703](https://github.com/user-attachments/assets/719ce1cf-1455-473e-947d-6eacf9d99651)


In some ticketing systems, users can set their own SLA preferences; however, in osTicket, SLA management is typically reserved for agents and managers.

---

---

## Conclusion

This README provides detailed instructions for setting up and managing an osTicket system, from post-installation configurations to ticket lifecycle management. Following these steps ensures a well-organized, efficient support workflow capable of handling critical issues effectively.

---


