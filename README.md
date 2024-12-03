ServiceNow Business Rule Implementation
This repository contains the documentation and implementation details for creating and testing a Business Rule in ServiceNow. The goal of this task is to demonstrate the use of business rules to automate the creation of related Problem records from high-priority Incidents.

Contents:
Overview
Steps to Implement
Result
File Details
Overview
A Business Rule in ServiceNow is a server-side script that runs whenever a record is inserted, updated, deleted, or queried. In this task:

A Business Rule is created on the Incident table.
The rule is triggered after inserting or updating an incident with Priority: 1 - Critical.
It automatically creates a related Problem record with the same short description as the incident.
Steps to Implement
Create a Business Rule:

Set the Name to After br -1.
Apply the rule to the Incident table.
Ensure the rule runs after insert or update operations.
Add the necessary filter conditions for Priority: 1 - Critical.
Add the Script:

Use the provided script to automate the creation of a related Problem record.
Test the Rule:

Create a new incident with Priority: 1 - Critical and submit it.
Verify that a new Problem record is automatically created.
Result
When an incident with Priority: 1 - Critical is created or updated:
A corresponding Problem record is generated.
The Problem record inherits the short description from the incident.
