# Week 1 - Project Setup & Planning

This journal documents the progress made during the first week of BALTRA's development.

---

## Day 1 · Development Environment Setup

**Date:** 2026-07-08

### Goals

- Set up the development environment.
- Create the initial project structure.
- Configure Git and GitHub.
- Install PostgreSQL.
- Create the first project documentation.

### Completed

- Verified Python, Git and Node.js installation.
- Installed PostgreSQL 17.
- Created the GitHub repository.
- Initialized the local Git repository.
- Created the project folder structure.
- Added the first project documentation.
- Performed the first commit.
  
### Decisions

- Project name: **BALTRA**.
- Meaning: **BALance + TRAck**.
- Main goal: build a professional full-stack expense tracker that resembles a real SaaS product rather than a university assignment.

### Lessons Learned

- A well-prepared development environment prevents future issues.
- Version control should be configured before writing any code.
- Good project organization is as important as the implementation itself.

### Next steps

- Define product vision.
- Gather requirements.
- Design the system architecture.
- Create the initial GitHub Project board.

---

# Day 2 – Product Vision & Planning

**Date:** 2026-07-24

## Goals

- Define the vision of BALTRA.
- Plan the development roadmap.
- Establish the main phases of the project.
- Define the scope of the first version.

## Completed

- Created the Project Vision document.
- Created the Project Roadmap.
- Defined the MVP features.
- Planned the different development phases.

## Decisions

- The project will focus on delivering a complete and polished MVP before adding advanced features.
- The application will follow a structured development process, similar to a real software project.
- Future features will be planned separately to keep version 1.0 focused.

## Lessons Learned

- Planning the project before coding helps define clear objectives.
- A roadmap makes it easier to organize the work and track progress.
- Defining the MVP helps avoid adding unnecessary features too early.

## Next Steps

- Write the project requirements.
- Design the software architecture.
- Create the database design.
---

# Day 3 – Project Requirements

**Date:** 2026-07-25

## Goals

- Define the functional requirements.
- Define the non-functional requirements.
- Write the user stories.
- Define the scope of version 1.0.

## Completed

- Created the requirements document.
- Defined the functional requirements.
- Defined the non-functional requirements.
- Wrote the user stories.
- Defined the features that are out of scope.

## Lessons Learned

- Functional requirements describe what the application must do.
- Non-functional requirements describe how the application should behave.
- User stories help describe the application from the user's point of view.

## Next Steps

- Design the software architecture.
- Plan the database structure.
- Design the REST API.

---

# Day 4 – Software Architecture

**Date:** 2026-07-25

## Goals

- Design the overall architecture of BALTRA.
- Define the main components of the application.
- Understand how the frontend, backend and database communicate.
- Create the first architecture diagram.

## Completed

- Created the software architecture document.
- Defined the responsibilities of the frontend, backend and database.
- Described how the different components communicate.
- Created the system architecture diagram.

## Lessons Learned

- A client-server architecture separates the frontend, backend and database into independent components.
- The frontend communicates with the backend through a REST API.
- The backend is responsible for processing requests and interacting with the database.
- Designing the architecture before coding makes the project easier to develop and maintain.

## Next Steps

- Design the database.
- Define the REST API.
- Start the backend development with FastAPI.

---

# Day 5 – Database Design

**Date:** 2026-07-25

## Goals

- Design the database structure.
- Identify the main entities and their relationships.
- Create the Entity-Relationship Diagram (ERD).
- Make design decisions for the first version of BALTRA.

## Completed

- Created the database design document.
- Defined the User, Expense and Category entities.
- Designed the relationships between the tables.
- Created the ER diagram using draw.io.
- Decided to use global categories for version 1.0.

## Design Decisions

- Categories will be shared by all users in the first version of the application.
- The database follows a simple relational model to keep the MVP easy to develop and maintain.
- Future versions may allow users to create their own custom categories.

## Lessons Learned

- A primary key uniquely identifies each record in a table.
- A foreign key creates a relationship between two tables.
- Planning the database before coding helps avoid future problems and makes the application easier to extend.

## Next Steps

- Design the REST API.
- Start setting up the backend with FastAPI.