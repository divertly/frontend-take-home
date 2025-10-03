# Frontend Take Home Project


#### The purpose of this project is to gauge your technical skills and ability to design and implement a well-functioning, performant, and maintainable frontend application. The goal is not to waste your time or have you do work for us for free -- your take home project does not have any practical use for our products. 

## Brief
Please create a column-based To Do application, similar to a JIRA Kanban or Trello board, to be viewed and interacted with in a web browser. Once the project is complete, please open a PR against this repo for us to review. 

### Please do not spend too many hours working on this project -- we're more interested in how you work and solve problems than we are perfection

### Feature Requirements
* Every To Do should default to 3 columns: To Do, Doing, and Done.
* Each todo should exist on a "card" and cards should be able to be dragged and dropped between columns.
* Each card should have a Title and Description
* Users should be able to create and delete cards as necessary
* Uses should be able to create and delete columns as necessary
* Each card should have a direct link to it, so that going to "myapp.com/todo/<cardID>" displays the card title and description

### Design Considerations
* Because there's no backend, feel free to use whatever storage you think is best (browser state, etc.)
* You have full design and UI creativity -- we want to see your creativity alongside your technical ability!

# Frontend Take Home Project

This project evaluates your frontend skills and approach to building maintainable, testable applications. We want to see how you design, implement, and iterate—using Test-Driven Development (TDD) as the primary workflow.

IMPORTANT: We expect work to follow TDD. That means: write tests first, make them fail, implement the smallest change to make them pass, then refactor. Tests are not optional—show us your process through test commits and clear test suites.

## Brief
Create a column-based To Do application (like a Kanban board) to be viewed and interacted with in a browser. When finished, open a Pull Request (PR) against this repo for review.

Please don't spend excessive time—we're evaluating your thinking and process as much as the final product.

## TDD Expectations (what we're looking for)
- Write tests before implementing features. Use small, focused tests that document intended behavior.
- Include tests that fail initially and then pass after your implementation—this demonstrates TDD.
- Provide at least one test for each core feature (examples below).
- Keep tests fast and deterministic. Prefer unit tests for logic and small integration tests for component behavior.
- Add meaningful commit messages that show the test -> implementation -> refactor cycle when possible.

Contract (simple)
- Inputs: Browser interactions / JSON fixtures for todos and columns
- Outputs: UI state, data persistence (browser storage), and router links
- Error modes: invalid input, empty titles/descriptions, drag/drop edge-cases

Edge cases we expect tests or thought about
- Creating a card with empty or very long title/description
- Dragging a card to an empty column or to the same column
- Deleting a column that contains cards (and deciding what happens to the cards)
- Direct link to a card that doesn't exist

## Feature Requirements
- App defaults to 3 columns: To Do, Doing, Done.
- Todo items are displayed on cards; cards can be dragged and dropped between columns.
- Each card has a Title and Description.
- Users can create and delete cards.
- Users can create and delete columns.
- Each card has a direct link (e.g. `/todo/<cardID>`) that displays that card's title and description.

## Design Considerations
- No backend is required—use browser state or any client-side storage you prefer (localStorage, indexedDB, in-memory, etc.).
- We want to see thoughtful UI/UX decisions. Design is part of the evaluation.

## Technical Notes
- Do not use AI code generation tools (Copilot, ChatGPT, Claude, etc.). We want to see your code.
- Use any framework (React, Vue, Svelte, Solid, or none). Choose what lets you show your best work.
- Tests are required and are evidence of your TDD workflow. We don't require 100% coverage, but include several meaningful tests.

Quality gates we suggest you cover in your PR (helps reviewers):
- Build succeeds (include scripts to install and run),
- Lint/type checks (if applicable),
- Unit tests and at least one small integration test demonstrating core UI behavior,
- Short README instructions to run the app and the tests.

## How to show your TDD workflow in your submission
- Make small commits that show tests being added first and then implementation.
- Include a README section (or commit notes) describing the testing strategy and what each test verifies.
- If you used a particular testing library (Jest, Vitest, Testing Library, Cypress, Playwright, etc.), list it and show how to run tests.

## Example commands (add the corresponding scripts to your project)
These are example commands—adapt them to your project's tools and package manager.

```bash
# install deps (example)
npm install

# run the app (example)
npm start

# run tests (example)
npm test
```

## Process
When complete, open a PR against this repository. Be prepared to talk through your design decisions, testing approach, trade-offs, and potential next steps.

If you have questions, contact your recruiter.

Thanks, and happy TDD-driven coding!
