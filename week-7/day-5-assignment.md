#### Objective

Deploy `proxy-key` to Render and use it to call a key based API without exposing the key in your front end source code.

#### Requirements

1. Fork `https://github.com/tm-LBenson/proxy-key` and deploy it to Render as a Web Service.
2. Add one environment variable in Render such as `key`, `key2`, `key3`, `key4`, or `key5`.
3. From your front end app, make a `POST` request to your deployed `proxy-key` endpoint and use the returned key to call one API that requires a key.
4. Render the API result in the page and show loading and error states.
5. README includes your live URL and explains that the key is not committed to GitHub or hard coded in your client code.

#### Notes

This is for learning only. It is not a secure production API. Do not use paid API keys here. Roll or delete your key when you are done.

#### Submission

Git repo link [live URL if applicable]

#### Rubric (20 pts)

- Meets the objective 0-5
- Render deployment works 0-5
- Key is not exposed in front end source 0-5
- Project runs from README 0-5
