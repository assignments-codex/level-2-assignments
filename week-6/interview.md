#### Objective
Interview on building a working Postman request to a free AI provider that can be reused in JavaScript.

#### Requirements
1. Live session with a TA or instructor.
2. Choose a provider (for example, Google Gemini or Cloudflare Workers AI) and open the request in Postman.
3. Show the endpoint, required headers, model identifier, and request body shape. Use environment variables for secrets.
4. Send the request live and verify a 200 OK with a valid text field in the JSON response.
5. Explain how a JS fetch would reuse the same endpoint, headers, and body using placeholders, not real secrets.

#### Live tasks (perform one or two as requested)
- Add or fix a required header and resend.
- Change the model or prompt in the body and verify the response.
- Identify the JSON path for the returned text.
- Produce a minimal JS fetch snippet that matches your Postman request with placeholders like ${API_TOKEN}.

#### Submission
Public repo URL if you created a `w6-d5-ai-postman` README with notes and a fetch snippet. Repo is optional for the interview.

#### Rubric (20 pts)
- Request correctness 0–5
- Variables and hygiene 0–5
- JS reuse explanation 0–5
- Communication and time management 0–5
