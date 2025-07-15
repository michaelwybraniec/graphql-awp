# Agentic Workflow Protocol (AWP)

## Init

1. This Agentic Workflow Protocol (AWP) governs collaboration between human and AI contributors. The following principles must always be followed:

    1.1. All work is guided strictly by the AWP; no deviations or improvisation.

    1.2. The AI must always listen to the human, never override instructions, and never take initiative beyond what is explicitly requested.

    1.3. Every change or decision must be validated by the human before proceeding.

    1.4. The AI must never hide changes or actions; transparency is required at all times.

    1.5. If instructions from the human are unclear, the AI must ask clarifying questions and never assume or anticipate requirements.

    1.6. The protocol is designed to ensure trust, clarity, and effective collaboration between human and AI.

## Author

1. Overvibing.com community

## Goal

1. The main objective of this project is to develop a production-ready GraphQL application with a solid, well-documented schema, a seeded database for testing, robust authentication and validation, automated testing, a demonstration client, comprehensive documentation, and clear deployment instructions—ensuring the app is reliable, maintainable, and ready for real-world use.

## Overview

1. This project aims to build a production-ready GraphQL application from the ground up. The process is organized into main phases, each representing a key milestone in the journey toward a robust and maintainable codebase. By following best practices for schema design, security, testing, and deployment, we ensure that each milestone builds upon the previous, resulting in a fully functional API and client, ready for real-world use.

    1.1. Build a production-ready GraphQL API with a well-structured, documented schema.

    1.2. Use a seeded database (JSON file for simplicity) to enable development and testing.

    1.3. Implement authentication and basic authorization for API endpoints.

    1.4. Provide robust input validation and error handling.

    1.5. Include automated tests for schema and resolvers, starting early and updating as features are added.

    1.6. Offer a simple client app to demonstrate and test the API.

    1.7. Generate and maintain up-to-date API documentation throughout development.

    1.8. Supply deployment instructions and environment configuration for easy setup.

## Outcome

1. Success for this project is defined as:

    1.1. A fully functional, production-ready GraphQL API with a well-documented and robust schema.

    1.2. A seeded database (using a JSON file or similar) that enables reliable development and testing.

    1.3. Authentication and authorization implemented and working as intended.

    1.4. Comprehensive input validation and error handling throughout the API.

    1.5. Automated tests covering schema, resolvers, and key workflows, with all tests passing.

    1.6. A simple client application that demonstrates and validates the API’s capabilities.

    1.7. Up-to-date, clear documentation for both the API and the client.

    1.8. Easy-to-follow deployment instructions and environment configuration.

    1.9. Security best practices are followed, with sensitive data protected and basic protections in place.

    1.10. Codebase is organized, maintainable, and extensible, with clear contribution guidelines.

    1.11. Basic performance considerations are addressed, and the API is efficient for typical use cases.

    1.12. CI/CD workflows are in place for linting, testing, and deployment.

    1.13. Basic logging and error monitoring are implemented or documented.

    1.14. The client app is accessible and user-friendly.

    1.15. A clear license file and, if applicable, community guidelines are provided.

    1.16. All work and changes have been validated by the human, with full transparency and adherence to the Agentic Workflow Protocol.

    1.17. All decisions and changes are traceable, with an escalation path for blockers or disagreements.

## Collaboration

1. **ai_agent_senior_developer:**  Senior Developer (AI Agent)

2. **ai_agent_junior_developer:**  Junior Developer (AI Agent)

3. **ai_agent_designer:**  Designer (AI Agent)

4. **ai_agent_tester:**  Tester (AI Agent)

5. **ai_agent_documentation:**  Documentation (AI Agent)

6. **ai_agent_project_manager:**  Project Manager (AI Agent)

7. **ai_agent_product_owner:**  Product Owner (AI Agent)

8. **ai_agent_scrum_master:**  Scrum Master (AI Agent)

9. **human_developer:**  Developer (Human)

10. **human_designer:**  Designer (Human)

11. **human_tester:**  Tester (Human)

12. **human_documentation:**  Documentation (Human)

13. **human_project_manager:**  Project Manager (Human)

14. **human_product_owner:**  Product Owner (Human)

15. **human_scrum_master:**  Scrum Master (Human)

16. **approver:** Human Only (Human)

17. **approval_timeout:**  10 minutes

18. **auto_handoff:**  true

## Steps

- [ ] 1. Project Initialization
    - [x] 1.1: Create initial README.md based on the project objectives written in AWP.md"
    - [ ] 1.2: Set up project structure with PostGraphile
    - [ ] 1.3: Create initial project documentation
    - [ ] 1.4: Set up development environment
    - [x] 1.5: init a first Commit to Git repository

- [ ] 2. GraphQL Schema Design
    - [ ] 2.1: Define initial GraphQL schema
    - [ ] 2.2: Document schema structure
    - [ ] 2.3: Create JSON seed data
    - [ ] 2.4: Set up database connection

- [ ] 3. Authentication & Authorization
    - [ ] 3.1: Implement authentication mechanism
    - [ ] 3.2: Add basic authorization checks
    - [ ] 3.3: Create user roles and permissions

- [ ] 4. API Development
    - [ ] 4.1: Implement GraphQL resolvers
    - [ ] 4.2: Add input validation
    - [ ] 4.3: Create error handling mechanisms

- [ ] 5. Testing
    - [ ] 5.1: Set up testing framework
    - [ ] 5.2: Write unit tests for schema
    - [ ] 5.3: Write resolver tests
    - [ ] 5.4: Create integration tests

- [ ] 6. Client Application
    - [ ] 6.1: Develop simple client to demonstrate API
    - [ ] 6.2: Implement basic UI
    - [ ] 6.3: Test API interactions

- [ ] 7. Documentation
    - [ ] 7.1: Generate API documentation
    - [ ] 7.2: Create README with setup instructions
    - [ ] 7.3: Document deployment process

- [ ] 8. CI/CD & Deployment
    - [ ] 8.1: Set up CI/CD workflows
    - [ ] 8.2: Configure deployment environment
    - [ ] 8.3: Add basic logging and monitoring

## Notes

1. Technology Stack:
   - PostGraphile: Automatic GraphQL API generation from PostgreSQL
   - PostgreSQL: Primary database
   - MIT Licensed, Open-Source Technology

2. Key Technology Considerations:
   - Leverage PostGraphile's automatic schema generation
   - Implement Row-Level Security (RLS)
   - Focus on type-safety and performance
   - Use PostgreSQL's built-in authentication mechanisms

3. Development Philosophy:
   - Prioritize database-first approach
   - Minimize custom resolver logic
   - Maximize use of PostgreSQL's native capabilities

4. Performance Targets:
   - Aim for efficient query execution
   - Minimize N+1 query problems
   - Implement caching strategies

5. Security Focus:
   - Implement strict input validation
   - Use PostgreSQL's role-based access control
   - Protect sensitive data through database-level permissions

## Procedures

1. **update**

    1.1. Review README.md and AWP.md after each step.

    1.2. Update README.md to reflect the current state

    1.3. We review AWP.md to understand next actions.

    1.4. Check for blockers, if any we notify humans.

    1.5. Ensure docs and code are aligned, of not, notify humans.

2. **commit**

    2.1. Commit changes using the commitStandard.

    2.2. Use the format: type(scope step): subject.

    2.3. Reference the step number in every commit message.

    2.4. Follow conventional commit standards.

    2.5. Include relevant files.

3. **next**

    3.1. Move to the next actionable step only after update and commit are complete.

    3.2. Identify the next actionable step and begin work.

    3.3. Check for blockers before proceeding, and confirm additional plan with human.

    3.4. Mark the current step as done before you start.

4. **check**

    4.1. Review AWP.md to determine the current actionable step.

    4.2. Find the first step not done.

    4.3. Restore context and understand what needs to be done.

    4.4. Use this when returning to work after a break or context loss.

5. **handoff**

    5.1. Transfer task ownership between human and AI.

    5.2. Package current context and deliverables.

    5.3. Notify receiving party with clear expectations.

    5.4. Set timeout for response and escalation rules.

## Notes

1. 

2. 

3. 

4. 

5. 

## Commit Standard

1. **format:** type(scope step): subject

2. **types:** feat, fix, docs, test, chore

3. **rules:**

    3.1. Reference the step in every commit.

    3.2. Use imperative mood.

    3.3. Keep messages concise and descriptive.

4. **examples:**

    4.1. feat(api 3.1): add API endpoint

    4.2. docs(readme 5.1): expand documentation
