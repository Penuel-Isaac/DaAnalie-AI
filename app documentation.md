 📊 DaAnalie AI – API Documentation

Overview
DaAnalie is an intelligent AI-powered hiring platform that uses machine learning to analyze resumes, rank candidates, and recommend top talent.


📡 API Endpoints

1. *Register User*
*POST* `/api/auth/register`

json
{
  "firstName": "John",
  "lastName": "Doe",
  "email": "john@example.com",
  "password": "StrongPass123!"
}



2. *Verify Email*
*POST* `/api/auth/verify`

json
{
  "email": "john@example.com",
  "code": "123456"
}



3. *Login*
*POST* `/api/auth/login`

json
{
  "email": "john@example.com",
  "password": "StrongPass123!"
}


4. *Submit Applicant*
*POST* `/api/applicants/submit`

json
{
  "fullName": "Jane Doe",
  "resume": "base64 or file URL",
  "skills": ["Python", "SQL"],
  "experience": 3
}


 5. Get Ranked Candidates (Admin)
GET /api/applicants/ranked

Response: List of ranked candidates.