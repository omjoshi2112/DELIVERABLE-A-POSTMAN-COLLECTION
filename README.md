# Task --04
COMPANY NAME: CODTECH IT SOLUTION PVT.LTD

NAME: OM JOSHI

INTER ID: CT6WKCL.

DOMAIN: SOFTWARE TESTING.

BATCH DURATION: January 5th,2025 to February 20TH,2025.

MENTOR NAME: NEELA SANTHOSH

DESCRIPTION: PERFORM ADVANCED LOAD TESTING OF A WEB APPLICATION USING GATLING. 

Steps for Advanced Load Testing with Gatling

Set Up Gatling
Download Gatling from gatling.io.
Ensure Java (JDK 8+) is installed.

Write the Load Test Script
Create a Scala script in user-files/simulations.

Define:
Base URL: Application URL.

Scenarios: User actions (e.g., login, data fetch).

Load Profile: User ramp-up and duration.

Example: 
setUp(
  scenario("Load Test")
    .exec(http("Homepage").get("/"))
    .exec(http("Login").post("/login").formParam("user", "test").formParam("pass", "1234"))
    .inject(rampUsers(1000).during(60))
)
Execute ./bin/gatling.sh and select your script.Analyze Results

Review the generated HTML report for metrics like response time, throughput, and errors.
-----------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------
**DELIVERABLE: A DETAILED REPORTON SYSTEM PERFORMANCE UNDER SIMULATED HEAVY LOADS**

Deliverable: Detailed Performance Report

Overview
Test setup details: tools, load test objectives, and scenarios tested (e.g., login, data retrieval).
Test Scenarios

Describe user actions simulated (e.g., ramping 1000 users over 60 seconds).Include load configuration details (e.g., users, duration).

Performance Metrics
Response Time: Average, min, max.

Throughput: Requests per second.

Error Rate: Percentage of failed requests.

CPU/Memory Usage: Server resource utilization (if monitored).

Analysis of Results
Identify bottlenecks (e.g., slow pages, high error rates).Compare performance against expected thresholds.

Conclusion & Recommendations
Summarize system behavior under heavy load. Suggest optimizations or infrastructure scaling if necessary.Include Visuals

Charts and graphs showing key metrics (response time trends, user load vs. performance).
