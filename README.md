# JMeter API Performance Testing

## Overview

This project demonstrates API performance testing using Apache JMeter against the JSONPlaceholder REST API.

The objective was to evaluate API response times, throughput, and stability under concurrent user load while validating successful responses through response assertions.

## Tools Used

* Apache JMeter 5.6.3
* JSONPlaceholder REST API
* GitHub

## Test Configuration

### Load Profile

| Parameter               | Value      |
| ----------------------- | ---------- |
| Virtual Users           | 50         |
| Ramp-Up Period          | 10 Seconds |
| Loop Count              | 5          |
| Total Requests Executed | 250        |

### API Tested

**Method:** GET

**Endpoint:** https://jsonplaceholder.typicode.com/posts

## Test Components

* Thread Group
* HTTP Request Sampler
* Response Assertions
* Summary Report
* Aggregate Report
* HTML Dashboard Report

## Assertions Implemented

### Response Validation

* HTTP Status Code Validation
* Expected Response Code: 200
* Error Monitoring

## Performance Results

| Metric                | Result             |
| --------------------- | ------------------ |
| Total Samples         | 250                |
| Average Response Time | 251 ms             |
| Median Response Time  | 83 ms              |
| 90th Percentile       | 304 ms             |
| Throughput            | 19 Requests/Second |
| Error Rate            | 0%                 |

## Key Findings

* API remained stable throughout the test execution.
* All requests completed successfully with 0% errors.
* Average response time remained within acceptable limits.
* Throughput reached approximately 19 requests per second.
* Response validation confirmed successful API responses.

## Repository Structure

```text
jmeter-api-performance-testing/

├── README.md
├── json_placeholder.jmx
├── aggregate_report.jtl
└── report/
    ├── index.html
    ├── statistics.json
    ├── content/
    └── sbadmin2-1.0.7/
```

## Skills Demonstrated

* Performance Testing
* Load Testing
* API Testing
* Response Validation
* JMeter Test Plan Creation
* Assertions
* Throughput Analysis
* Response Time Analysis
* Performance Metrics Reporting

## Author

QA Engineer with experience in Manual Testing, API Testing, Database Testing, Performance Testing, and Automation Testing.
