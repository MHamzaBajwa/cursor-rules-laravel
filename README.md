# HTMX Cursor Rules for Modern Web Applications

This project provides a set of guidelines and best practices for using [HTMX](https://htmx.org/) to build interactive, maintainable, and efficient web applications. The rules are designed for developers who want to leverage HTMX's power to enhance user experience without heavy reliance on JavaScript.

## Key Principles
- **Concise and Clear Code:** Write technical responses with precise HTMX examples.
- **Enhanced Interactivity:** Use HTMX to add interactivity directly in HTML, minimizing JavaScript.
- **Maintainability:** Prioritize clean, readable, and maintainable code in both frontend and backend.
- **Descriptive Attributes:** Use clear and descriptive HTMX attribute names for better collaboration.

## HTMX Usage Guidelines
- Use `hx-get`, `hx-post`, and other HTMX attributes to define server requests in HTML.
- Structure server responses to return only the necessary HTML snippets for updates.
- Favor declarative HTMX attributes over JavaScript event handlers.
- Leverage `hx-trigger` to control when requests are sent based on user actions.
- Use `hx-target` to specify where response content is injected in the DOM.

## Error Handling and Validation
- Implement server-side validation for data integrity.
- Return appropriate HTTP status codes (4xx, 5xx) and user-friendly error messages.
- Use `hx-swap` to customize how responses (including errors) are inserted into the DOM.

## Dependencies
- [HTMX (latest version)](https://htmx.org/)
- Any backend framework (Django, Flask, Node.js, etc.) to handle server requests.

## HTMX-Specific Guidelines
- Use `hx-confirm` to prompt users before critical actions (e.g., deletions).
- Combine HTMX with frontend libraries like Bootstrap or Tailwind CSS for enhanced UI.
- Use `hx-push-url` to update the browser's URL without a full page refresh.
- Organize templates to serve reusable HTMX fragments efficiently.

## Performance Optimization
- Minimize server response sizes by returning only essential HTML.
- Implement server-side caching for frequently requested HTMX endpoints.
- Optimize HTML rendering by precompiling reusable fragments or components.

## Key Conventions
1. Follow consistent naming conventions for HTMX attributes.
2. Prioritize fast and intuitive user experiences.
3. Maintain a modular template structure for clarity and manageability.
