# Coursify Development Journal

## Day 1 – August 27, 2025
- ✅ Created new GitHub repo `coursify`  
- ✅ Initialized project with `README.md`  
- ✅ Added `.gitignore` for Node.js setup  
- 📝 Planned initial scope of the project  

**Reflection:** Solid start — repo is live and basic structure is in place. Ready to begin development iterations.

---

## Day 2 – August 28, 2025
- ✅ Set up `connectDB` utility with async/await and error handling  
- ✅ Integrated MongoDB connection in `index.js`  
- 🤔 Learned difference between `await connectDB()` vs just `connectDB()` in server setup  

**Reflection:** Made good backend progress — database connection working. Cleared up async/await usage questions, which boosted confidence in handling async workflows.

---
## Day 3 – August 29, 2025
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