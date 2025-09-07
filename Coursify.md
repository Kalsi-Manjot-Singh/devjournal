# Coursify Development Journal

## 📅 Day 1 – August 27, 2025
- ✅ Created new GitHub repo `coursify`  
- ✅ Initialized project with `README.md`  
- ✅ Added `.gitignore` for Node.js setup  
- 📝 Planned initial scope of the project  

**Reflection:** Solid start — repo is live and basic structure is in place. Ready to begin development iterations.

---

## 📅 Day 2 – August 28, 2025
- ✅ Set up `connectDB` utility with async/await and error handling  
- ✅ Integrated MongoDB connection in `index.js`  
- 🤔 Learned difference between `await connectDB()` vs just `connectDB()` in server setup  

**Reflection:** Made good backend progress — database connection working. Cleared up async/await usage questions, which boosted confidence in handling async workflows.

---

## 📅 Day 3 – August 29, 2025
- ✅ Implemented User Signup
  - Added Zod validation for `name`, `email`, `password`, and `role`
  - Normalized empty role strings to default to `'student'`
  - Hashed passwords with bcrypt before saving
  - Generated JWT access token on successful signup
- ✅ Updated User schema
  - Added `trim: true` to string fields
  - Added default value for `role`
- ✅ Connected signup controller to `/signup` route

**Reflection:** Signup flow is now fully functional with proper validation and token generation. Excited to implement login next and continue building the authentication system.

---

## 📅 Day 4 - September 06, 2025
- ✅ Implemented User Login
  - Normalized emails to prevent duplicates
  - On Login, Credentials are validated with bcrypt compare
  - Security Note: Returning a single "Invalid Credentials" for both bad emails and
  passwords to avoid enumeration attacks.

**Reflection:** I now have a working MVP for an auth system

📝 Next step: add input validation for login using zod and refactor repetitive code into small utilities

---


## 📅 Day 5 - 08 Sept 2025 – Error Handling System
	•	Implemented a custom AppError class for consistent error structure.
	•	Built a global errorMiddleware to handle errors based on environment (development vs production).
	•	Integrated Zod validation with detailed error reporting (.issues).
	•	Refactored controllers (signup and login) to throw AppError consistently.
	•	Verified that validation errors, operational errors, and server errors are all handled gracefully.

**Reflection:** ✅ Codebase is now much cleaner and has a robust error-handling foundation.

📝 Next step: Centralize zod validation for DRY and implement it in login as well
---
