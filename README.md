# Unexpected Multiple useEffect Triggers in Next.js 15 App

This repository demonstrates an unexpected behavior in a Next.js 15 application where the `useEffect` hook in a component triggers multiple times after the initial render, even though the dependency array is correctly set.  This is a simple counter example, however, the issue could happen in various scenarios.

## Bug Description

The About page's counter increments as expected, but the console log within the `useEffect` hook shows multiple renders after the initial one.  This leads to unnecessary re-renders and can potentially cause performance issues or unexpected behavior.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to the `/about` page.
5. Click the increment button several times and observe the console logs.

## Solution

The issue is resolved in the `solution` branch using strict mode. While not always the solution, it addresses this particular instance.  See the `solutionContent` for a more detailed explanation.