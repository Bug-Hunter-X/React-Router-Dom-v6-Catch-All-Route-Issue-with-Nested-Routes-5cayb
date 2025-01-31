# React Router v6 Catch-All Route Bug

This repository demonstrates a subtle bug in React Router v6 related to the catch-all route (`/*`) when used in conjunction with nested routes.  The catch-all route unexpectedly intercepts all navigation, even when a more specific route should match.

## Bug Description

The issue arises when a catch-all route (`/*`) is defined alongside other routes, particularly when nested routes are involved.  Even if a nested route is a better match, the catch-all route will always be activated.  This is inconsistent with the expected behavior of more specific routes having priority.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Navigate to any route; the catch-all route will always be displayed.

## Solution

The solution involves carefully considering the order of routes and using nested routes strategically.  The provided `bugSolution.js` demonstrates the correct way to handle this scenario.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.