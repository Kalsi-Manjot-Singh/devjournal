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

## Day 5 – July 23, 2025
- Completed **onboarding process API docs** in detail  
- Thorough documentation of request payloads and flows  
- Set foundation for later automation bot phases  

**Reflection:** Slowed down on coding to really document everything — this will pay off when flows get more complex.

## Day 6 – July 28, 2025
- Initiated **Hinge onboarding process automation**  
- First code scaffolding for sequential onboarding steps  
- Added retries + better structure for API calls  

**Reflection:** The automation journey truly begins — setting up resilience for flaky endpoints.

## Day 7 – July 31, 2025
- Finished **email verification flow**  
- Integrated Mail.tm for disposable emails  
- Token + account verification working end-to-end  

**Reflection:** Email OTP step complete — one of the bigger blockers out of the way!

## Day 8 – August 1, 2025
- Built **random date generator utility** for Date of Birth step  
- Implemented DOB submission to `/user/v3` + flow update  
- Added better logging around profile state fetch  

**Reflection:** Small step but important — onboarding flow is filling out piece by piece.

## Day 9 – August 4, 2025
- Added **proxy manager + geolocation utilities**  
- Integrated IP-based location into onboarding payloads  
- Ensured location consistency across profile setup  

**Reflection:** Routing traffic via proxies makes the bot far more realistic — groundwork for scaling.

## Day 10 – August 6, 2025
- Implemented multiple onboarding steps:
  - Children (Don’t have children)  
  - Ethnicity (White/Caucasian)  
  - Relationship type (monogamy)  
- Added flow updates + logging for each  

**Reflection:** Knocked out 3 profile fields in one day — momentum is building!

## Day 11 – August 7, 2025
- Added onboarding steps:
  - Drinking, tobacco, marijuana usage  
  - Education, politics, religion  
- Integrated **flow sync + visibility flags**  
- Started **user flow metrics integration** (screen refs 17–23)  

**Reflection:** The profile setup is getting close to parity with the real Hinge app.

## Day 12 – August 8, 2025
- Refactored onboarding into **context-driven architecture**  
- Shared run context (`ctx`) carrying axios, headers, token, geo, etc.  
- Split flow into phases:
  - `otpFlow.js`  
  - `profileSetup.js`  
  - `finalize.js`  
- Improved **email OTP reliability** (extended retries, logging)  

**Reflection:** Huge refactor day — modular architecture will keep the project maintainable.