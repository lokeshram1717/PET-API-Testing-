🧪 PetStore API Testing with Postman, Newman & Jenkins CI/CD

🚀 Overview -
This project demonstrates end-to-end API automation testing using Postman, Newman, and Jenkins CI/CD integration.
It covers automated testing of the Swagger PetStore API, including test creation, validation, report generation, and continuous integration setup.

🧰 Tech Stack -

1.Postman – for designing and running API requests
2.Newman – Postman’s command-line tool for automation
3.HTML Extra Reporter – for generating detailed HTML reports
4.Jenkins – for CI/CD pipeline execution
5.Git & GitHub – for version control and repository management

🧩 Features Implemented

✅ Created a Postman collection for:
  a.Creating, retrieving, updating, and deleting pets in the Swagger PetStore
  b.Dynamic environment variable handling
  c.Retry mechanism for 404 responses (auto re-execution logic)
✅ Exported the Postman collection and environment for Newman execution
✅ Automated execution using Newman CLI
✅ Added delay handling and retry logic for real-world API sync issues
✅ Generated beautiful HTML Extra Reports
✅ Integrated with Jenkins for automated test runs
✅ Published the test report directly in Jenkins UI
✅ Linked the complete project with GitHub for version control

🔄 Jenkins Job Flow

1.Jenkins fetches the latest project files
2.Executes Newman command:
**newman run PetStore_API_Testing.postman_collection.json -e PetStore.postman_environment.json -r htmlextra --reporter-htmlextra-export report.html**
3.Waits between requests to ensure API stability
4.Publishes HTML Extra report under “HTML Report” tab in Jenkins
5.Implemented smart retry logic in Request Pet to handle 404s gracefully

📊 Reports

1.The project generates:
2.Newman HTML Extra Report → report.html
3.Stored and viewable via Jenkins HTML Publisher plugin

🧠 Learning Outcomes

Through this project:
1.Understood end-to-end API automation workflow
2.Gained hands-on experience with CI/CD integration for testing
3.Learned Git & GitHub version control fundamentals
4.Built reusable and maintainable Postman collections

🌐 Future Enhancements

1.Add CI pipeline with GitHub webhooks
2.Integrate Slack/Email notifications for test runs
3.Migrate collections into a Docker container for scalable runs
