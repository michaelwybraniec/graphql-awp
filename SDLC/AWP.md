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

## Project Backlog

- [ ] 1. Project Initialization
    - [x] 1.1: Create initial README.md based on the project objectives written in AWP.md"
    - [ ] 1.2: Set up project structure with PostGraphile
        - [x] 1.2.1: Choose the project structure (monorepo, single repo, folder layout, etc.)
            - Task: Evaluate and select the optimal project structure for a PostGraphile-based GraphQL API with a demo client
            - Options considered: Single-repo, Monorepo, Backend-with-client-subfolder
            - Decision: Backend-focused structure with client subfolder for clear separation
        - [x] 1.2.2: Initialize the project (e.g., npm/yarn init, set up package.json)
            - Task: Create the basic folder structure and initialize Node.js projects
            - Actions: Create /api and /client directories, run npm init -y in each
            - Outcome: Both directories have package.json with default values
        - [ ] 1.2.3: Install PostGraphile and required dependencies
            - Task: Install core PostGraphile dependencies in the /api folder
            - Dependencies to install: postgraphile (GraphQL API generator), pg (PostgreSQL client)
            - Command: npm install postgraphile pg
            - Purpose: Enable automatic GraphQL schema generation from PostgreSQL
        - [ ] 1.2.4: Set up a basic server entry point (e.g., index.js/ts)
            - Task: Create the main server file that will run PostGraphile
            - File: /api/src/index.js or /api/index.js
            - Content: Basic Express server with PostGraphile middleware
            - Purpose: Provide a working server that can start and serve GraphQL API
        - [ ] 1.2.5: Create a folder for database seed and config files
            - Task: Organize database-related files and configurations
            - Folders to create: /api/db, /api/config
            - Files: Database connection config, seed data structure
            - Purpose: Separate database concerns and prepare for data seeding
        - [ ] 1.2.6: Add a placeholder for the GraphQL schema (if needed)
            - Task: Create structure for custom GraphQL schema extensions
            - Folder: /api/schema or /api/graphql
            - Purpose: Prepare for custom resolvers or schema modifications beyond PostGraphile's auto-generation
        - [ ] 1.2.7: Add scripts to start the server and run PostGraphile
            - Task: Update package.json with useful npm scripts
            - Scripts: "start", "dev", "build" (if needed)
            - Purpose: Provide easy commands to run the development server
        - [ ] 1.2.8: Update README.md to reflect the new structure and setup instructions
            - Task: Document the project structure and how to get started
            - Content: Folder structure explanation, setup steps, basic usage
            - Purpose: Ensure anyone can understand and run the project
        - [ ] 1.2.9: Commit the initial project structure
            - Task: Save all changes to git with appropriate commit message
            - Message format: feat(structure 1.2.x): description of changes
            - Purpose: Track progress and maintain version control
    - [ ] 1.3: Create initial project documentation
        - Task: Create comprehensive documentation for the project setup and development process
        - Files to create: CONTRIBUTING.md, DEVELOPMENT.md, API.md
        - Content: Development guidelines, API documentation, contribution workflow
        - Purpose: Ensure team members and contributors understand how to work with the project
    - [ ] 1.4: Set up development environment
        - Task: Configure development tools and environment variables
        - Actions: Set up .env files, configure linting (ESLint), add .gitignore
        - Files: .env.example, .eslintrc.js, .gitignore
        - Purpose: Ensure consistent development environment across team members
    - [x] 1.5: init a first Commit to Git repository
        - Task: Initialize git repository and make first commit
        - Actions: git init, git add, git commit
        - Purpose: Establish version control and track project history

- [ ] 2. GraphQL Schema Design
    - [ ] 2.1: Define initial GraphQL schema
        - Task: Design the core GraphQL schema structure for the application
        - Actions: Define types, queries, mutations, and subscriptions
        - Files: /api/schema/schema.graphql or database schema files
        - Purpose: Establish the foundation for all GraphQL operations
    - [ ] 2.2: Document schema structure
        - Task: Create comprehensive documentation for the GraphQL schema
        - Actions: Document types, fields, arguments, and relationships
        - Files: /docs/schema.md, GraphQL documentation
        - Purpose: Help developers understand and use the API effectively
    - [ ] 2.3: Create JSON seed data
        - Task: Generate sample data for development and testing
        - Actions: Create JSON files with realistic test data
        - Files: /api/db/seed-data.json, /api/db/seed.js
        - Purpose: Provide consistent test data and enable development without live data
    - [ ] 2.4: Set up database connection
        - Task: Configure PostgreSQL connection and database setup
        - Actions: Set up connection pool, configure environment variables
        - Files: /api/config/database.js, .env files
        - Purpose: Enable PostGraphile to connect to and read from PostgreSQL

- [ ] 3. Authentication & Authorization
    - [ ] 3.1: Implement authentication mechanism
        - Task: Set up user authentication system using PostgreSQL and JWT
        - Actions: Implement login/logout, JWT token generation, password hashing
        - Files: /api/auth/auth.js, /api/middleware/auth.js
        - Purpose: Secure the API and identify authenticated users
    - [ ] 3.2: Add basic authorization checks
        - Task: Implement role-based access control and permission checks
        - Actions: Create authorization middleware, check user permissions
        - Files: /api/middleware/authorization.js, /api/config/permissions.js
        - Purpose: Control access to different API endpoints based on user roles
    - [ ] 3.3: Create user roles and permissions
        - Task: Define user roles and their associated permissions
        - Actions: Create role definitions, permission mappings, database tables
        - Files: /api/db/migrations/roles.sql, /api/config/roles.js
        - Purpose: Establish clear permission structure for different user types

- [ ] 4. API Development
    - [ ] 4.1: Implement GraphQL resolvers
        - Task: Create custom resolvers for complex business logic beyond PostGraphile's auto-generation
        - Actions: Implement custom resolvers, optimize query performance
        - Files: /api/resolvers/, /api/schema/resolvers.js
        - Purpose: Handle complex queries and business logic not covered by PostGraphile
    - [ ] 4.2: Add input validation
        - Task: Implement comprehensive input validation for all GraphQL operations
        - Actions: Add validation middleware, create validation schemas
        - Files: /api/validation/, /api/middleware/validation.js
        - Purpose: Ensure data integrity and prevent invalid data from entering the system
    - [ ] 4.3: Create error handling mechanisms
        - Task: Implement robust error handling and logging throughout the API
        - Actions: Create error classes, implement error middleware, add logging
        - Files: /api/errors/, /api/middleware/error-handler.js
        - Purpose: Provide clear error messages and maintain system stability

- [ ] 5. Testing
    - [ ] 5.1: Set up testing framework
        - Task: Configure testing environment with Jest and GraphQL testing tools
        - Actions: Install testing dependencies, configure Jest, set up test database
        - Files: /api/jest.config.js, /api/tests/setup.js
        - Purpose: Enable automated testing of GraphQL schema and resolvers
    - [ ] 5.2: Write unit tests for schema
        - Task: Create comprehensive unit tests for GraphQL schema validation
        - Actions: Test type definitions, field resolvers, schema introspection
        - Files: /api/tests/schema/, /api/tests/unit/
        - Purpose: Ensure schema integrity and catch breaking changes early
    - [ ] 5.3: Write resolver tests
        - Task: Test custom resolvers and business logic
        - Actions: Mock dependencies, test resolver functions, validate outputs
        - Files: /api/tests/resolvers/, /api/tests/mocks/
        - Purpose: Verify resolver behavior and prevent regressions
    - [ ] 5.4: Create integration tests
        - Task: Test complete API workflows and end-to-end scenarios
        - Actions: Test authentication flows, database operations, error scenarios
        - Files: /api/tests/integration/, /api/tests/e2e/
        - Purpose: Ensure the entire system works together correctly

- [ ] 6. Client Application
    - [ ] 6.1: Develop simple client to demonstrate API
        - Task: Create a basic web client to showcase and test the GraphQL API
        - Actions: Set up React/Vue.js project, configure GraphQL client (Apollo Client)
        - Files: /client/src/, /client/package.json, /client/graphql/
        - Purpose: Provide a user-friendly interface to test and demonstrate API functionality
    - [ ] 6.2: Implement basic UI
        - Task: Create user interface components for API interaction
        - Actions: Build forms, data display components, navigation
        - Files: /client/src/components/, /client/src/pages/
        - Purpose: Enable users to interact with the API through a visual interface
    - [ ] 6.3: Test API interactions
        - Task: Verify client can successfully communicate with the GraphQL API
        - Actions: Test queries, mutations, error handling, authentication
        - Files: /client/src/tests/, /client/cypress/ (if using Cypress)
        - Purpose: Ensure the client application works correctly with the API

- [ ] 7. Documentation
    - [ ] 7.1: Generate API documentation
        - Task: Create comprehensive API documentation with examples and usage guides
        - Actions: Generate GraphQL documentation, create API reference, add examples
        - Files: /docs/api.md, /docs/examples/, GraphQL Playground setup
        - Purpose: Help developers understand and integrate with the API
    - [ ] 7.2: Create README with setup instructions
        - Task: Update main README with complete setup and usage instructions
        - Actions: Add installation steps, configuration guide, usage examples
        - Files: README.md, /docs/setup.md
        - Purpose: Enable new developers to quickly get started with the project
    - [ ] 7.3: Document deployment process
        - Task: Create deployment guides for different environments
        - Actions: Document production deployment, environment configuration, CI/CD setup
        - Files: /docs/deployment.md, /docs/environment.md
        - Purpose: Ensure smooth deployment to production and staging environments

- [ ] 8. CI/CD & Deployment
    - [ ] 8.1: Set up CI/CD workflows
        - Task: Configure automated testing, linting, and deployment pipelines
        - Actions: Set up GitHub Actions, configure automated testing, add deployment scripts
        - Files: /.github/workflows/, /scripts/deploy.sh
        - Purpose: Automate quality checks and deployment processes
    - [ ] 8.2: Configure deployment environment
        - Task: Set up production and staging deployment environments
        - Actions: Configure hosting platform (Heroku, AWS, etc.), set up environment variables
        - Files: /config/production.js, /config/staging.js, deployment scripts
        - Purpose: Enable reliable and repeatable deployments
    - [ ] 8.3: Add basic logging and monitoring
        - Task: Implement application logging and basic monitoring
        - Actions: Add logging middleware, configure monitoring tools, set up error tracking
        - Files: /api/middleware/logging.js, /api/config/monitoring.js
        - Purpose: Monitor application health and debug issues in production

## Unplanned Tasks

1. **Detailed Task Descriptions Added (2024-01-XX)**
   - Added comprehensive task descriptions for all steps in sections 1-8
   - Each task now includes: Task description, Actions, Files, and Purpose
   - Provides complete visibility and control over development process
   - Enables ultimate insight into what each step involves and why it's necessary

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

    3.4. Mark the current step 'check' [ ] as done before you start.

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
