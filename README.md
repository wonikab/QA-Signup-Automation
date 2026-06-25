# QA Signup Automation

## Overview
This automates the signup flow for the Authorized Partner website using Playwright.

Website:
https://authorized-partner.vercel.app/

## Technology Used

- JavaScript
- Playwright
- Node.js

## Prerequisites

- Node.js installed
- Playwright installed

## Installation

Open the project folder and run:

```bash
npm install
```

## Run the Test

```bash
npx playwright test tests/signup.spec.js --project=chromium --headed
```

## Notes

- The script automates the complete signup flow.
- A unique email address is generated automatically for each execution.
- The test pauses at the OTP verification step using `page.pause()`.
- Enter the OTP manually from Yopmail, click **Verify Code**, then click **Resume** in the Playwright Inspector.