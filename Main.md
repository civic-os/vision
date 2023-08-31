# Civic OS: Open Source Software to Empower Open Governance
Last Revised 2023-08-30

## Contact
For more information, or to collaborate, contact [Dan Kurin](mailto:dkurin@swiftlet.technology)

## Guiding Principles
### Open Government
Transparency and accountability are foundational to successful democratic governance. In order for citizens to be informed, they must have ready access to information to make good decisions about who to support, and how to vote in elections and on referenda.

In Civic OS, accountability is achieved by enforcing the justification of decisions; in other words, forcing leaders to justify key decisions. In order for an individual to decide if he supports an action, he must be able to understand the rationale behind that decision.
### Open Data
All data is not created equal. In order to make data open and usable the Open Data Charter has published [6 key
principles](https://opendatacharter.net/principles/):
- Open By Default
- Timely and Comprehensive
- Accessible and Usable
- Comparable and Interoperable
- For Improved Governance & Citizen Engagement
- For Inclusive Development and Innovation
### Open Source
The term “open source” can have a number of meanings but Civic OS uses the definition consistent with “free software” according to the [Free Software Foundation](https://www.fsf.org/about/what-is-free-software).

The two primary outcomes of this philosophy are democratic development and lower cost of entry. Democratic development allows entities to contribute to development (in code, financial, and administrative contributions) to influence the system’s evolution. This results in a system that is useful for a broad range of diverse organizations. Lower cost of entry is realized by the $0 licensing fees inherent in Free/Open Source software. When development is performed in the open, the cost is shared by an entire community.

## Goals
### Raise the level of abstraction
We believe that most information systems or processes can be abstracted in a way that a non-technical person can describe it if provided with the right tools. Similarly, the system for storing this information should allow that same non-technical person to understand and (most critically) contribute to the system's creation.
### Tools, not Products
Civic OS is a tool designed to allow experts in the information domain to create and maintain information systems without writing software code. As such, the system will not be complete without input from the organization operating the system but rather a completed system is created using Civic OS.
### Runs anywhere
This software is created to allow any organization to setup and administer their own instance of the application. You own the data and the software.

## Abstractions
To accommodate breaking a system into components, we propose the following abstractions. Every abstraction can be thought of as a computing primitive (in the vein of a "File" or "Folder") which may have configurable properties, but can be represented by a graph or diagram to visually represent its construction. These graphs are a key enabler to bridge the gap between technical and non-technical ideas and persons.
### Schema
A Schema is a structured set of information in a tabular form (having multiple records of the same type). A single schema comprises a collection of fields, each with a type (text, number, money, etc.) and relationships to other schemas or nested sub-schemas. Validity rules are also configurable to enforce data input and preserve data integrity (e.g. required fields, `End Date` must be after `Start Date`).

Every Schema is described by an Entity Relationship Diagram.
```mermaid
erDiagram

```
Every Schema may have a number of configurable properties that alter its behavior.
#### Permissions
Permissions define who can view records and who can edit records. For example:
- Functional permissions
  - Owner of record can edit
  - Anyone can view records marked as "Complete"
- Role-based permissions
  - Members of the `Road Crew` role can view `Work Order` records
  - Members of the `Dispatch` role can create `Schedule` records
#### Audit Log
When a record is updated, a log is automatically created to note the changed values as well as the user who made the update.
#### Search
Specific fields may be configured to make records easily searchable.
### Workflow

### Events/Triggers


## Governance
The Civic OS software is designed to maximize civic benefit, which should direct the legal structure of the supporting organization. This organization has not yet been formed, but we believe that a non-profit or Public Benefit Corp. will provide the best opportunities to mature and spread the use of Civic OS.
### Representation
### Decision-making

## Technical Implementation
### User Experience
### Software Architecture