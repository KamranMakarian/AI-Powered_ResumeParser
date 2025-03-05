# Functional Requirements (User Stories)

1. **As a user, I want to submit a resume in text format so that the system can parse and store the applicant's information.**
   - Endpoint: `POST /api/applicant`
   - Requires authentication: No
   
2. **As an authenticated user, I want to view all parsed resumes so that I can analyze the stored applicant data.**
   - Endpoint: `GET /api/applicants`
   - Requires authentication: Yes (`USER`, `ADMIN` roles)
   
3. **As an authenticated admin, I want to update an applicant's information using their ID so that the data remains current and accurate.**
   - Endpoint: `PUT /api/applicant/id/{id}`
   - Requires authentication: Yes (`ADMIN` role only)
   
4. **As a user, I want to search for applicants by their role so that I can find candidates suitable for a specific position.**
   - Endpoint: `GET /api/applicants/role/{roleName}`
   - Requires authentication: Yes (`USER`, `ADMIN` roles)
   
5. **As a user, I want to retrieve all the roles associated with a particular applicant by their ID so that I can assess their suitability for different roles.**
   - Endpoint: `GET /api/roles/{applicantId}`
   - Requires authentication: Yes (`USER`, `ADMIN` roles)


