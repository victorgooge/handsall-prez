# Zoku_Testing_Proposal.docx

**Proposal: Dedicated “Testing” Category for Campus-Based QA**
Private Zoku testing deployment for QA interns to validate location-based flows around Georgia State University.

| **Audience** | **Core idea** | **Primary outcome** |
| ---| ---| --- |
| QA + Backend | Add a private “Testing” category that behaves like a normal category but routes testers to GSU-tailored locations. | Make it easier for interns to test the full clue flow on physical phones with realistic, accessible campus destinations. (Ease of access and convenience) |

**Overview**
For the private QA deployment, introduce a category named “Testing” in the app UI. This category should behave like the normal categories and activities already in Zoku, follow the same overall user flow, and guide testers through location-based experiences tailored to places around the GSU campus.
The goal is not to create a separate test harness or shortcut flow. The goal is to let testers experience the real in-app journey on physical devices — from category selection, to activity selection, to clue progression, to destination discovery — using accessible campus locations that are easy for our interns to reach.
![](https://t9013785310.p.clickup-attachments.com/t9013785310/4cc7605f-5cec-4298-8de6-4c4fc8c55a8e/25bcc557-55fc-4a06-9494-391df4a95aa1.png)![](https://t9013785310.p.clickup-attachments.com/t9013785310/17b7d115-b865-43b8-94ad-a20717a59cc7/9527d84b-8cfd-4424-92a2-8ae7e27b8083.png)**Current Testing Methods:**
![](https://t9013785310.p.clickup-attachments.com/t9013785310/2940811d-ea8e-40e4-be53-80162cb916a8/ec68f781-11d5-458f-b40e-d195f0e0d24b.png)
*   _External Testing Panel (Custom)_
*   _Android Virtual Device Location Control Panel_
**Current Limitations:**
*   Does not account for location fetching and tracking in real time
*   Lots of latency
*   Tedious
**Advantages – Deployment vs. Simulation**
*   Most of our interns are GSU students, so campus-based destinations make testing more convenient and repeatable.
*   It gives QA a realistic way to validate location tracking, GPS accuracy, clue progression, and map behavior on physical phones.
*   It lowers the friction of testing while still preserving the same user experience and navigation flow we want in production.
*   It creates a controlled environment for catching issues in First Clue → Second Clue → Proximity Search without needing random off-campus destinations.
**Requested backend update**
*   Create backend support for a “Testing” category that mirrors the current category/activity structure as closely as possible.
*   Seed this category with testing activities tailored to GSU campus locations or nearby student-accessible spots.
*   Keep the same downstream behavior as standard activities so the app exercises the real location-based clue flow instead of custom one-off logic.
**Suggested testing activity locations**
*   Campus buildings or classrooms
*   Libraries, plazas, or recognizable landmarks
*   Food spots or quick meetup locations near campus
NOTE: The actual venue does not matter. The main idea here is to ensure clue functions are working properly, getting users from point A to point B

**Dashboard placement reference**
The screenshot below is the current dashboard design reference where the “Testing” category would be added.
![](https://t9013785310.p.clickup-attachments.com/t9013785310/c577d69d-4b33-44bb-8273-f2e2890083b8/image.png)
“Testing” category to be added in development environment/deployment
_Dashboard screen reference for the proposed “Testing” category placement._

**Conclusion**
*   Furthermore, a supported testing environment will greatly help to validate a majority of test cases.
**Next Steps**
Victor – Frontend:
*   Share all documents with testers: Upload overview file
*   Give testers access to GitHub Organization to access repositories
*   Finalize in-depth testing guidelines
    *   Provide feature details, requirements, demos, and diagrams
    *   Refine test cases
    *   Clarify deliverables
Ike – Backend + Data Entry:
*   Currently setting up backend database to support testing
*   Assigning tester roles
Hema, Eka, Vivana – QA Testers:
*   Join GitHub Org
*   Work on getting application deployed and available on physical devices through TestFlight