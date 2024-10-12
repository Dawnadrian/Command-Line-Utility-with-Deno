# Command-Line-Utility-with-Deno
creating a clu practicing the syntax of deno,js and the tdd approach:

Programming Exercise: Building a Command-Line Utility with Deno
Objective: Create a command-line utility cm (comment manager) to manage a list of topics and comments associated with those topics. This exercise will help you strengthen your familiarity with JavaScript and Deno, while practicing Test-Driven Development (TDD) and organizing functionality using Models and Controllers.

Features to be made:
1. Add a Topic: Users can create new topics.
Command: cm topic add <topic-name>

2. List Topics: Users can list all available topics.
Command: cm topic list

4. Add a Comment: Users can comment on a specific topic.
Command: cm comment add <topic-name> <comment-text>

5. List Comments for a Topic: Users can list comments under a specific topic.
Command: cm comment list <topic-name> --sort [asc|desc]
**Comments should be sortable by their creation dates, either in ascending (asc) or descending (desc) order.

6. Delete a Comment: Users can delete a comment based on its ID.
Command: cm comment delete <topic-name> <comment-id>
Persistence: Store the topics and their comments using Deno KV to persist data between command executions.

Structure:
Models: Represent the data entities (Topics and Comments).
Controllers: Manage business logic, interacting with models and Deno KV for persistence.
CLI Interface: Parse commands and route them to the appropriate controller.
TDD Approach:
Write tests first for each command feature (e.g., adding a topic, adding a comment, sorting comments, etc.).
Implement each feature and refactor iteratively.
