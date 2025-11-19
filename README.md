# 💳 FinTech E-Wallet – Bill Payment Error Breakdown (Power BI & PowerPoint)

## 📌 Project Overview

This project analyzes the decline in bill payment success rate on an e-wallet app since August 2023, using transactional, session, event log, and error data.
The analysis applied the MECE framework to break down the payment journey (authentication, gateway, app version, user flow) and identify the most critical failure points.

 Power BI was using for calculation and chart creation, and a PowerPoint report for business storytelling.

## 🚀 Analytical strategy design
Use MECE (Mutually Exclusive, Collectively Exhaustive) to split the problem into components.
<img width="3045" height="2750" alt="whiteboard_exported_image" src="https://github.com/user-attachments/assets/68e9f173-4272-4379-9d6b-2d208565ef28" />


## 🎯 Objectives

- Measure the drop in success rate and its business impact.
- Identify failure points across the user payment journey.
- Assess the effect of app version updates and gateway downtime during peak/off-peak hour
- Recommend short-term actions to stabilize reliability.
- 
Key slides: Problem Definition → Objectives → Error Analysis → Insights → Short-term Solutions.

## 📊 Key Insights

- Success Rate Decline: Payment success fell from 91.7% in July → 86.9% in August despite a increase in transaction volume.
- Billing Category Impact: The billing category (36.65% of payments) suffered the largest drop (−14.6% success rate), driving most of the decline.
- Payment Journey Drop-offs:
Select Payment Type → Enter Amount: −17% drop.
View Receipt: −17.6% drop (post-payment, UX issue)
- Error Drivers:
   1. Wallet balance failures up +6.08%, led by insufficient balance and limit exceedance.
   2. Authenticator errors (3D Secure timeout & invalid OTP) = >75% of authentication failures.
   3. API timeouts peaked at midnight & off-peak hours, not just high traffic periods.
   4. App version 3.9.6–3.9.9 showed consistent declines in success, with rising partner errors.
   4. Gateway downtime surged 0.32% → 0.72% in late August.

  ## 📸 Dashboard & Report Preview
<img width="1327" height="754" alt="Screenshot 2025-11-19 105849" src="https://github.com/user-attachments/assets/46b03d67-b74a-454c-82fc-4aa17fe5c274" /> 
<img width="1332" height="759" alt="Screenshot 2025-11-19 105901" src="https://github.com/user-attachments/assets/24e2f562-d15f-412a-9177-d9f1b59c49eb" /> 
<img width="1327" height="759" alt="Screenshot 2025-11-19 105910" src="https://github.com/user-attachments/assets/da092401-11da-40fb-a4c7-ef2fe68d0dbb" />
<img width="1333" height="757" alt="Screenshot 2025-11-19 105919" src="https://github.com/user-attachments/assets/61e3b827-3824-4b91-a392-eb0c170a35d6" />
<img width="1339" height="757" alt="Screenshot 2025-11-19 105929" src="https://github.com/user-attachments/assets/86e55414-8488-4d59-8679-54fd07cdfb2d" />
<img width="1337" height="753" alt="Screenshot 2025-11-19 105938" src="https://github.com/user-attachments/assets/7e9dd044-4f39-4560-9e78-a7cbad6828d1" />
<img width="1322" height="750" alt="Screenshot 2025-11-19 110004" src="https://github.com/user-attachments/assets/da0f35ba-c699-4944-b071-c330b6e13d3c" />
<img width="1343" height="754" alt="Screenshot 2025-11-19 110012" src="https://github.com/user-attachments/assets/8d9bd0cb-561a-48d5-a2fb-49b26fee27dc" />
<img width="1327" height="755" alt="Screenshot 2025-11-19 110024" src="https://github.com/user-attachments/assets/15d0035d-a763-4c7b-b749-6f0bf944ebdf" />
 
  ## ✅ Short-term solution Recommendation

- **Balance & Limit Alerts** – Real-time notifications before payment (e.g., balance < $50).
- **UX Optimization** – Simplify payment type selection flow to reduce drop-offs.
- Authentication Fixes – Introduce **Smart OTP / email OTP** to reduce 3D Secure failures.
- Gateway Reliability – **Deploy backup servers** to avoid single points of failure.
- App Version QA – Strengthen regression testing before release to prevent sharp declines.

## 🌍 Use Cases

- Product Managers – Prioritize fixes by business impact.
- Engineering Teams – Address API & authenticator stability.
- Operations & Risk – Manage partner downtime and wallet funding errors.
- Executives – Understand financial & customer experience risks.

## 🛠️ Tools & Methodology

- Power BI Desktop – Data modeling and visualization.
- MECE Framework – Structured breakdown of error categories.
- PowerPoint – Executive storytelling of findings & solutions.




