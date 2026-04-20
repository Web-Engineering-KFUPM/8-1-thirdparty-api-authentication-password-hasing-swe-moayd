# 8-1-Thirdparty-API-Authentication-Password-Hasing — Feedback

## Submission

- **Lab:** 8-1-Thirdparty-API-Authentication-Password-Hasing
- **Deadline (Riyadh / UTC+03:00):** 2026-04-20T20:59:00+03:00
- **Last commit time (from git log):** 2026-04-20T08:46:54Z
- **Submission marks:** **20/20** (On time)


## Files Checked

- Repo root (cwd): /Users/moaydshahat/8-1-thirdparty-api-authentication-password-hasing-swe-moayd
- Grader directory: /Users/moaydshahat/8-1-thirdparty-api-authentication-password-hasing-swe-moayd/script
- Detected project root: /Users/moaydshahat/8-1-thirdparty-api-authentication-password-hasing-swe-moayd
- server.js: ✅ /Users/moaydshahat/8-1-thirdparty-api-authentication-password-hasing-swe-moayd/server.js

---

## TODO-by-TODO Feedback

### TODO 1: POST /register — **28/28**

**Checklist**
- ✅ Defines POST route for "/register"
- ✅ Reads req.body or destructures email/password from req.body
- ✅ Validates missing email/password
- ✅ Returns 400 for missing email/password
- ✅ Handles duplicate registration somehow
- ✅ Uses bcrypt.hash(...) to hash password
- ✅ Stores user with email and password hash
- ✅ Returns 201 on successful registration
- ✅ Has register error handling

**Deductions / Notes**
- ✅ No deductions. Good job!

### TODO 2: POST /login — **26/26**

**Checklist**
- ✅ Defines POST route for "/login"
- ✅ Reads req.body or destructures email/password from req.body
- ✅ Handles user lookup / missing user case
- ✅ Uses bcrypt.compare(...)
- ✅ Returns wrong-password response
- ✅ Creates JWT using jwt.sign(...)
- ✅ Uses JWT secret "abc123" or JWT_SECRET in jwt.sign
- ✅ Uses expiresIn "1h" or equivalent
- ✅ Returns token response
- ✅ Has login error handling

**Deductions / Notes**
- ✅ No deductions. Good job!

### TODO 3: GET /weather — **26/26**

**Checklist**
- ✅ Defines GET route for "/weather"
- ✅ Reads Authorization header
- ✅ Returns 401 when token/header is missing
- ✅ Extracts bearer token
- ✅ Verifies JWT using jwt.verify(...)
- ✅ Returns invalid-token response
- ✅ Reads city from req.query.city
- ✅ Returns city-required response
- ✅ Builds some external weather API URL using the city
- ✅ Uses fetch(...) to call weather API
- ✅ Checks weather API response status
- ✅ Parses JSON from weather API
- ✅ Returns some structured weather response
- ✅ Has weather error handling

**Deductions / Notes**
- ✅ No deductions. Good job!

---

## How marks were deducted (rules)

- JS comments are ignored, so starter TODO comments do NOT count.
- The grader checks only `server.js`.
- Manual Postman testing is NOT graded.
- npm install commands and setup instructions are NOT graded.
- Checks are intentionally lenient and verify top-level implementation only.
- Code can be in ANY order; repeated code is allowed.
- Common equivalents are accepted where possible.
- Missing required items reduce marks proportionally within that TODO.
- Exact formatting is not required as long as the core coding logic is present.
- For the weather TODO, any reasonable public weather/geocoding API structure is accepted.
