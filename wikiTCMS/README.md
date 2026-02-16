# hiWikiTCMS

leverage wikiTCMS (wiki Test Case Management System) as TestLink replacement for hierarchied QA process: 
    Test Plan/ 
        Test Case 
            /Test Run


```
You want a process where:

CI/CD runs normally:
Build → Unit Tests → Packaging → Deployment to staging/test environment
After that, a CQ (Code Quality) Gate runs:

Executes a specific test-case group (e.g., smoke, regression, API, performance, feature group)
Pulls test cases from your TMS (TestLink, Kiwi TCMS, Nitrate…)
Fails the pipeline if required test groups fail


Results persist across pipeline executions and feed into your QA approval flow.```

- docker-compose up -d
- docker exec -it kiwi_web /Kiwi/manage.py initial_setup
