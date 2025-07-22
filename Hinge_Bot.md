# Hinge Bot Development Journal

## Day 1 – July 17, 2025
- ✅ Setup Node.js project with `.env` and git
- ✅ Integrated DaisySMS for phone number provisioning
- 📝 Documented initial plan
**Reflection:** Groundwork is laid; ready to iterate fast.

## Day 2 – July 18, 2025
- Documented Hinge API endpoints in detail  
- Implemented initial device identity utility  
- Expanded logger utility for better debugging  
- Added `.gitignore` for cleanup

**Reflection:** Getting familiar with Hinge’s network flow; good progress documenting endpoints.

## Day 3 – July 21, 2025
- Added a dedicated **logger utility** and updated DaisySMS service to use it  
- Implemented **device identity utility** for generating Hinge API device headers  
- Cleaned up documentation and improved project organization  
- Added `.gitignore` adjustments  

**Reflection:** Starting to build a more solid foundation — logging and device identity will make the flow more realistic and easier to debug.

## Day 4 – July 22, 2025
- Built and tested **sendOTP function**  
- Implemented **sendInstallId()** for onboarding  
- Fixed rate-limiting issues from Hinge by tweaking device handling  
- Improved full logging for OTP submit + token store  
- Made edits to onboarding docs for clarity  

**Reflection:** OTP handling is critical — today’s progress means we can reliably get tokens and move deeper into the onboarding flow.