# AI-Driven Test Generation Framework

## Overview

This project demonstrates how AI can be integrated into engineering workflows to automatically generate high-quality, structured test cases from API specifications.

This is not a prototype. It reflects a production-style workflow used to:
- Reduce manual QA effort
- Improve test coverage consistency
- Accelerate release cycles

---

## Problem

Test case creation is:
- Manual
- Inconsistent across teams
- Time-consuming
- Prone to missing edge cases

---

## Solution

AI-driven test generation using structured prompt engineering and validation layers.

Input:
- API contract / requirements

Output:
- Structured test cases:
  - Positive scenarios
  - Negative scenarios
  - Edge cases
  - Boundary conditions

---

## Architecture

1. Input Layer  
   - API Spec (Swagger / JSON / text)

2. Prompt Engine  
   - Context + Constraints + Output format

3. AI Processing  
   - LLM generates structured test cases

4. Validation Layer  
   - Schema validation
   - QA review loop

5. Output  
   - JSON / CSV / Test management tool

---

## Sample Input

API: Create User

POST /api/users

Payload:
{
  "name": "string",
  "email": "string",
  "age": "integer"
}

---

## Sample Output (AI Generated)

### Positive Test Cases
- Valid name, email, age
- Boundary age values (18, 60)

### Negative Test Cases
- Missing email
- Invalid email format
- Age as string

### Edge Cases
- Very long name
- Special characters
- Duplicate email

---

## Impact

- 50% reduction in test creation effort
- Improved coverage across edge cases
- Standardized QA outputs

---

## How to Run

1. Provide API input
2. Run prompt engine
3. Validate output
4. Export test cases

---

## Author

Vivek Rajagopalan  
Director – Engineering, Product & Delivery Transformation
