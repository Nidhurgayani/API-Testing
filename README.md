# API Testing with Postman — JSONPlaceholder REST API

Designed and executed a full API testing project covering **GET, POST, PUT, PATCH, and DELETE** methods against the JSONPlaceholder REST API, using Postman.

## 📌 Objective

To apply structured API testing practices — functional validation, negative testing, and automated assertions — to a public REST API, simulating a real-world QA API testing workflow.

## 🛠 What Was Done

- Built a structured **Postman collection (20 requests)** organized into **Users**, **Negative Testing**, and **Posts** folders.
- Wrote and executed **20 test cases** covering positive testing, negative testing, status code validation, response body validation, query parameters, and header validation.
- Automated assertions using **Postman test scripts (pm.test)** for status codes and response content.
- Applied negative-testing techniques to uncover **3 real API inconsistencies** (e.g., malformed request bodies returning 500 instead of 400, and inconsistent handling of non-existent resource IDs across PUT/PATCH).
- Documented findings in a full **API Testing Report (PDF)** with a dedicated Bugs Found section, following standard bug-report structure (steps to reproduce, expected vs. actual, severity, impact).
- Tracked the project in **Jira** using an Epic → Story → Tasks structure, with individual Bug tickets for each defect.

## ✅ Results

| Metric | Count |
|---|---|
| Test Cases Executed | 20 |
| API Inconsistencies Found | 3 |
| HTTP Methods Covered | GET, POST, PUT, PATCH, DELETE |
| Pass Rate | 85% (17 PASS / 3 FAIL) |

## 🐞 Key Findings

| Bug ID | Description | Impact |
|---|---|---|
| BUG_API_001 | PUT on non-existent user ID returns 500 instead of expected error handling | High |
| BUG_API_002 | DELETE on non-existent user ID returns 200 instead of 404 | Medium |
| BUG_API_003 | Malformed JSON body on POST returns 500 instead of 400 | High |

## 📂 Repository Structure

```
├── 01-postman-collection/
│   └── Week5_API_Testing_Collection.json
├── 02-test-cases/
│   └── Week_5_API_Test_Cases.xlsx
├── 03-api-testing-report/
│   └── API_Testing_Report.pdf
├── 04-screenshots/
│   └── (Jira backlog, Jira board, Postman collection screenshots)
└── README.md
```

## 🧰 Tools Used

- Postman (collection design, pm.test automated assertions)
- Microsoft Excel (test case documentation)
- Jira (Epic → Story → Tasks → Bugs tracking)
- JSONPlaceholder REST API (test target)

## 🌐 API Under Test

[JSONPlaceholder](https://jsonplaceholder.typicode.com)

## 👤 About

This project is part of an ongoing self-directed QA learning journey, extending manual testing fundamentals into API testing — covering functional, negative, and validation testing on a public REST API.
