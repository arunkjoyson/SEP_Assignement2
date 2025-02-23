# Assignment 2: Requirements

### Student Details

**Name:** Arun Kanjirathingal Joyson  
**Student ID:** 8955136

---

### Problem Statement:

The AI developer client uses web scraping to collect training data for AI models. However, they face two main challenges:

- Developers want to have categorized training questions that are separate from the answers because developers care about self-affirmation.
- Developers want to know that the training data they are using is “balanced” (does not contain biases) because this will give them better AI models

---
# Q) Analysis of current 2 requirements: 

### Requirement 1: Categorized Training Questions & Answers

As an AI developer, I want training questions to be categorized separately from answers so that I can ensure self-affirmation.

## Assumption:

1. Developers benefit from self-affirmation when questions and answers are separated.

2. Categorization improves retrieval, filtering, and dataset usability.

## Validation:

- Ask developers how often they struggle with mixed question-answer data when using training datasets.[1]

- Do you think determining whether categorization improves searchability and organization in AI training?[2]

  - **Follow-Up Questions:**

    - What methods were tried before to organize?

    - What are the common categories you think are good?

- Do you actively use datasets with separate questions and answers to measure self-affirmation impact?[1]

- Do you think categorization is enough to fix this issue?[2]

## Preliminary Tasks:

- [ ] Identify common categories of training questions (e.g., programming, mathematics, general knowledge).

- [ ] Review existing training datasets to understand their current format and structure.

- [ ] Interview developers to assess whether question-answer separation improves their workflow.

- [ ] Explore possible UI/UX designs for a better categorization system.

- [ ] If categorization alone isn’t enough, identify the simplest technology to enhance organization.

## Metrics for Success:

- Accuracy of categorization: >95%.

- Processing Speed: Categorization time of <500ms per question.

- Developer Feedback: >80% satisfaction rate on data organization.

## Outcome:

- A structured system where training questions are categorized and separate from answers, improving usability for developers.

### Requirement 2: Balanced & Bias-Free Training Data  

As an AI developer, I want the training data to be balanced and free of biases so that I can build more reliable AI models.  

## Assumption:  

1. Unbalanced training data negatively affects AI model performance.  
2. Biases exist in web-scraped data and need mitigation.  

## Validation:  

- Do analysis of scraped training data to check for common biases (e.g., gender, racial, political biases).[1]  
  - **Follow-Up Questions:**  
    - What methods are currently used to detect biases in the training data?  
    - How frequently are biases identified in the current datasets?  

- Compare AI performance metrics before and after applying bias mitigation techniques.[1]
  - **Follow-Up Questions:**  
    - What specific performance metrics are used to evaluate AI models?  
    - How significant is the performance improvement after bias mitigation?  

- Gather feedback from developers on whether biased datasets have affected their previous models.[2]  
  - **Follow-Up Questions:**  
    - Can you provide examples of how biased data has impacted your models?  
    - What steps have you taken in the past to address these biases?  

## Preliminary Tasks:  

- [ ] Identify common sources of bias in scraped data.  
- [ ] Implement a bias-detection mechanism for automated flagging.  
- [ ] Review academic research on bias mitigation strategies.  
- [ ] Test small-scale AI models with and without bias correction.  
- [ ] Assess if manual review of flagged biases is necessary or if automation suffices.  

## Metrics for Success:  

- Bias Detection Accuracy: >90% in detecting bias.  
- False Positive Rate: <5% false positives.  
- Performance Consistency: <2% performance difference across groups.  

## Outcome:  

- A training dataset that minimizes biases and leads to improved AI model fairness and accuracy.

# Q) define some Requirements which will include both functional and system requirements.

### Functional Requirement 1: Automated Web Scraping Module  

As an AI developer, I want an automated web scraping module that retrieves publicly available data from diverse sources so that I can efficiently collect training data easily.  

## Assumptions:  
1. AI developers collect training data through web scraping.  
2. Web scraping is the most efficient method to gather large-scale training data.  
3. Publicly available data can be used without legal restrictions.  

## Validation:  

- How do you collect training data?[1]  
- Ask whether the current web scraping process is manual or semi-automated.[1]  
  - **Follow-Up Questions:**  
    - How is the current web scraping process managed? Is it fully manual, semi-automated, or automated?  
    - What are the main challenges faced with the current process?  

- Check if existing AI training workflows depend on external scraping tools.[2]  
  - **Follow-Up Questions:**  
    - Are there any specific external scraping tools currently in use? If so, which ones?  
    - How do these tools impact the overall AI training workflow?  

- Confirm compliance with data collection regulations (e.g., robots.txt, legal policies).[3]  
  - **Follow-Up Questions:**  
    - Are there any specific legal or ethical concerns related to the data sources being scraped?  
    - How is compliance with data collection regulations currently ensured?  

## Preliminary Tasks:  

- [ ] Define the key data sources that need to be scraped.  
- [ ] Research available scraping technologies and tools.  
- [ ] Implement a prototype to test data retrieval efficiency.  
- [ ] Address potential legal and ethical concerns regarding web scraping.  
- [ ] Evaluate the scalability of the module for high-volume data collection.  

## Metrics for Success:  

- **Efficiency:** Time taken to scrape data from each source should be reduced by 50%.  
- **Data Volume:** Ability to retrieve at least 1GB of data per hour from multiple sources.  
- **Error Rate:** Less than 2% error rate in data retrieval.  
- **Compliance:** 100% adherence to legal and ethical standards.  
- **Scalability:** Ability to handle a 100% increase in data volume without performance degradation.  

## Outcome:  

- An automated web scraping module that efficiently retrieves training data from multiple sources while ensuring compliance with legal and ethical standards.

### Functional Requirement 2: Configurable Scraping Parameters  

As an AI developer, I want the system to allow configurable scraping parameters so that I can control source selection and frequency.  

## Assumptions:  
1. Not all data sources are equally valuable, and developers need filtering options.  
2. Scraping frequency needs to be adjustable based on data availability and project needs.  

## Validation:  

- Gather feedback from developers on the most commonly needed filtering parameters.[1]  
  - **Follow-Up Questions:**  
    - What filtering parameters do you find most useful in your current workflow?  
    - How often do you need to adjust scraping parameters?  

- Determine whether frequent scraping causes redundant or unnecessary data collection.[2]  
  - **Follow-Up Questions:**  
    - Have you experienced issues with redundant data collection? If so, how often?  
    - How do you currently manage redundant or unnecessary data?  

- Assess if parameter customization improves data quality and reduces preprocessing effort.[2]  
  - **Follow-Up Questions:**  
    - How does parameter customization impact your data preprocessing efforts?  
    - Can you provide examples of how customized parameters have improved data quality?  

## Preliminary Tasks:  

- [ ] Identify key filtering parameters (e.g., keywords, categories, content type).  
- [ ] Implement a UI for configuring scraping settings.  
- [ ] Test different configurations to determine impact on data quality.  
- [ ] Optimize scheduling to balance data freshness and processing costs.  
- [ ] Ensure logs track all parameter changes for auditability.  

## Metrics for Success:  

- **Customization Flexibility:** Ability to configure at least 10 different scraping parameters.  
- **Data Quality:** >90% improvement in data relevance and quality.  
- **Redundancy Reduction:** <5% redundant data collected.  
- **Developer Satisfaction:** >85% satisfaction rate with the configurability of scraping parameters.  

## Outcome:  

- A flexible scraping system that allows developers to fine-tune data collection based on their needs.  

### Functional Requirement 3: Manual Review & Editing of Training Data  

As an AI developer, I want the system to allow manual review, editing, and removal of training data so that I can ensure only high-quality data is used for AI training.  

## Assumptions:  

1. Automated scraping may introduce errors, irrelevant content, or biased data.  
2. Manual review is necessary to refine training datasets.  

## Validation:  

- Analyze how often developers manually correct training data in existing workflows.[1]
  - **Follow-Up Questions:**  
    - How frequently do you manually review and correct training data?  
    - What types of errors or issues do you commonly encounter during manual review?  

- Compare model performance before and after manual data curation.[2]
  - **Follow-Up Questions:**  
    - How does manual data curation impact your model's performance?  
    - Can you provide examples of improvements seen after manual review?  

- Determine if automated pre-filtering can reduce the need for manual review.[2]  
  - **Follow-Up Questions:**  
    - Have you used automated pre-filtering before? If so, how effective was it?  
    - What additional features would improve automated pre-filtering for your needs?  

## Preliminary Tasks:  

- [ ] Design an intuitive UI for browsing and editing training data.  
- [ ] Implement permissions for who can review and edit data.  
- [ ] Test different approaches (e.g., automated flagging for review).  
- [ ] Log all modifications for transparency and rollback purposes.  

## Metrics for Success:  

- **Review Accuracy:** >95% accuracy in identifying and correcting errors.  
- **Processing Speed:** Manual review time <2 minutes per data entry.  
- **Developer Satisfaction:** >85% satisfaction rate with the review and editing process.  
- **Error Reduction:** >90% reduction in errors after manual review.  

## Outcome:  

- A system that enables developers to refine and curate high-quality AI training datasets.

### Functional Requirement 4: API for External AI Training Pipelines  

As an AI developer, I want the system to provide an API that integrates with external AI training pipelines so that I can automate data ingestion.  

## Assumptions:  

1. Developers prefer seamless integration with existing AI tools.  
2. Manually exporting/importing data slows down the workflow.  

## Validation:  

- Identify the most commonly used AI training platforms requiring integration.[1]
  - **Follow-Up Questions:**  
    - Which AI training platforms do you currently use?  
    - What integration features are most important to you?  

- Ensure API usability with different programming languages and frameworks.[1]
  - **Follow-Up Questions:**  
    - What programming languages and frameworks do you use for AI development?  
    - Have you encountered any issues with API usability in the past?  

- Test API speed, security, and reliability under heavy data loads.[2]
  - **Follow-Up Questions:**  
    - How do you measure API performance in your workflows?  
    - What security concerns do you have regarding API integration?  

## Preliminary Tasks:  

- [ ] Define API endpoints for data retrieval, submission, and updates.  
- [ ] Implement authentication and access control measures.  
- [ ] Provide documentation and examples for easy integration.  
- [ ] Test API performance with real AI training pipelines.  

## Metrics for Success:  

- **Integration Speed:** API integration time <1 hour for new platforms.  
- **Performance:** API response times <500ms for 95% of requests.  
- **Security:** 0 security breaches during testing.  
- **Developer Satisfaction:** >90% satisfaction rate with API usability and documentation.  

## Outcome:  

- A robust API that allows developers to integrate training data with their AI models seamlessly.  

### Functional Requirement 5: Audit Logging & Modification Tracking  

As an AI developer, I want the system to log all modifications and provide an audit trail for training data changes so that I can track data quality.  

## Assumptions:  

1. Training data modifications impact AI model performance and need traceability.  
2. Developers need to track changes to debug and refine datasets.  

## Validation:  

- Identify if developers currently struggle with tracking data modifications.[1]
  - **Follow-Up Questions:**  
    - How do you currently track modifications to your training data?  
    - What challenges do you face with the current tracking methods?  

- Determine if auditing improves dataset consistency and debugging. [2]
  - **Follow-Up Questions:**  
    - How has auditing impacted your ability to maintain dataset consistency?  
    - Can you provide examples of how auditing has helped in debugging issues?  

- Test the impact of detailed logs on system performance and usability.[1]  
  - **Follow-Up Questions:**  
    - How do detailed logs affect your system's performance?  
    - What features would improve the usability of audit logs for you?  

## Preliminary Tasks:  

- [ ] Design a logging mechanism that captures all data modifications.  
- [ ] Implement a search feature to filter logs by user, date, and action.  
- [ ] Evaluate different storage solutions for long-term logging.  
- [ ] Ensure compliance with industry best practices for data auditing.  

## Metrics for Success:  

- **Log Completeness:** 100% of key events captured.  
- **System Performance:** <5% performance overhead due to logging.  
- **Audit Efficiency:** Historical logs retrievable within 2 minutes.  
- **Developer Satisfaction:** >85% satisfaction rate with the logging and tracking system.  

## Outcome:  

- A transparent logging system that helps developers track and manage training data modifications efficiently.

### Functional Requirement 6: Search & Filtering for Training Data  

As an AI developer, I want the system to provide search and filtering capabilities based on metadata so that I can quickly find relevant training data.  

## Assumptions:  

1. Large datasets become unmanageable without proper filtering tools.  
2. Developers need advanced search options for efficient data retrieval.  

## Validation:  

- Analyze how developers currently search for training data.[2]  
  - **Follow-Up Questions:**  
    - How do you currently search for and retrieve training data?  
    - What challenges do you face with the current search and filtering methods?  

- Determine if search and filtering improve dataset usability and processing speed.[1]  
  - **Follow-Up Questions:**  
    - How has the implementation of search and filtering tools impacted your workflow?  
    - Can you provide examples of improvements in data retrieval efficiency?  

- Test the impact of different indexing methods on performance. [2]
  - **Follow-Up Questions:**  
    - What indexing methods have you tried, and how effective were they?  
    - What performance metrics do you use to evaluate indexing methods?  

## Preliminary Tasks:  

- [ ] Define key metadata attributes for filtering (e.g., date, source, category).  
- [ ] Implement a fast indexing system for efficient searching.  
- [ ] Develop an intuitive UI for advanced search features.  
- [ ] Test different filtering methods to balance accuracy and performance.  

## Metrics for Success:  

- **Search Speed:** Response times <1 second for 95% of queries.  
- **Search Accuracy:** >90% relevance in search results.  
- **Developer Satisfaction:** >85% satisfaction rate with search functionality.  

## Outcome:  

- A powerful search and filtering system that enables developers to access training data efficiently.

### System Requirement 1: Scalable Web Scraping Infrastructure  

As a system architect, I want the web scraping infrastructure to be scalable so that it can handle increasing data demands without performance degradation.  

## Assumptions:  

1. The volume of publicly available data will grow over time.  
2. The system must support parallel scraping for efficiency.  

## Validation:  

- Conduct load testing to determine the system’s current capacity.[1]  
  - **Follow-Up Questions:**  
    - What is the current capacity of the web scraping infrastructure?  
    - How does the system perform under varying levels of concurrent scraping requests?
    - Do you think this load will increase eventually?  

- Monitor performance under varying levels of concurrent scraping requests.[2]  
  - **Follow-Up Questions:**  
    - What performance metrics are used to monitor the system?  
    - How does the system handle peak data demands?  

- Benchmark against industry standards for scalable web scraping architectures.[1]  
  - **Follow-Up Questions:**  
    - What industry standards are used for benchmarking?  
    - How does the current infrastructure compare to these standards?  

## Preliminary Tasks:  

- [ ] Implement distributed scraping using multiple worker nodes.  
- [ ] Optimize request throttling to prevent IP blocking.  
- [ ] Integrate a queuing system for managing scraping jobs.  
- [ ] Use cloud-based storage for efficient data management.  

## Metrics for Success:  

- **Scalability:** Ability to handle a 100% increase in data volume without performance degradation.  
- **Performance:** Maintain response times under 2 seconds for 95% of requests.  
- **Error Rate:** Less than 1% error rate during peak loads.  

## Outcome:  

- A web scraping infrastructure capable of scaling dynamically based on data demand.  

### System Requirement 2: Data Preprocessing & Cleaning Pipeline  

As a system architect, I want an automated data preprocessing and cleaning pipeline so that I can ensure high-quality and structured data for AI training.  

## Assumptions:  

1. Raw scraped data may contain noise, duplicates, or incomplete information.  
2. A preprocessing step is necessary before feeding data into AI models.  

## Validation:  

- Compare raw scraped data with cleaned datasets to measure improvements.[1]  
  - **Follow-Up Questions:**  
    - What improvements are observed after preprocessing?  
    - How is the quality of the cleaned data measured?  

- Analyze the impact of preprocessing on AI model accuracy.[2]
  - **Follow-Up Questions:**  
    - How does preprocessing affect model accuracy?  
    - What metrics are used to evaluate the impact?  

- Test the efficiency of different cleaning techniques (e.g., deduplication, normalization).[2]  
  - **Follow-Up Questions:**  
    - Which cleaning techniques are most effective?  
    - How is the efficiency of these techniques measured?  

## Preliminary Tasks:  

- [ ] Implement a module for detecting and removing duplicate data.  
- [ ] Develop rules for filtering irrelevant or low-quality data.  
- [ ] Automate data formatting to match AI training requirements.  
- [ ] Log all preprocessing actions for auditability.  

## Metrics for Success:  

- **Data Quality:** >95% reduction in noise and duplicates.  
- **Processing Speed:** Preprocessing time <1 second per data entry.  
- **Model Accuracy:** >5% improvement in AI model accuracy after preprocessing.  

## Outcome:  

- A structured and high-quality dataset ready for AI training.

### System Requirement 3: Data Bias Detection & Balancing Mechanism  

As a system architect, I want a bias detection and balancing mechanism so that I can ensure AI training data is representative and fair.  

## Assumptions:  

1. Training data can contain biases that affect AI model performance. (IBM, 2023)  
2. Automated techniques can help identify and mitigate bias.  

## Validation:  

- Measure bias levels in existing datasets using statistical methods.[1]  
  - **Follow-Up Questions:**  
    - What statistical methods are used to measure bias?  
    - How significant are the biases in the current datasets?  

- Compare AI model outputs before and after applying bias mitigation techniques.[1]  
  - **Follow-Up Questions:**  
    - How do bias mitigation techniques affect model outputs?  
    - What metrics are used to evaluate the impact?  

- Conduct fairness testing using diverse input scenarios.[2]
  - **Follow-Up Questions:**  
    - What input scenarios are used for fairness testing?  
    - How is fairness measured in these scenarios?  
    - Do you think automated techniques can help identify and mitigate bias?

## Preliminary Tasks:  

- [ ] Implement algorithms to detect overrepresented or underrepresented categories.  
- [ ] Develop tools for rebalancing datasets through sampling techniques.  
- [ ] Provide reports summarizing bias metrics for developer review.  
- [ ] Test bias detection on real-world datasets.  

## Metrics for Success:  

- Bias Detection Accuracy: >90% in detecting bias.  
- False Positive Rate: <5% false positives.  
- Performance Consistency: <2% performance difference across groups.  

## Outcome:  

- A bias-aware dataset that enhances the fairness of AI models.

### System Requirement 4: Secure API for Data Access & Integration  

As a system architect, I want a secure API for data access and integration so that I can allow AI developers to retrieve and submit training data efficiently and securely.  

## Assumptions:  

1. AI developers need a structured way to interact with the training dataset.  
2. Unauthorized access to training data should be prevented.  

## Validation:  

- Ask: How do you retrieve and submit training data now?[1]  
- Perform security penetration testing on the API. [2]
  - **Follow-Up Questions:**  
    - What security measures are currently in place for the API?  
    - How often is penetration testing conducted?  
- Ensure API response times meet performance benchmarks.[2]  
  - **Follow-Up Questions:**  
    - What are the current API response times?  
    - How do these times compare to performance benchmarks?  
- Implement and test role-based access control mechanisms. [2] 
  - **Follow-Up Questions:**  
    - What role-based access controls are implemented?  
    - How effective are these controls in preventing unauthorized access?  

## Preliminary Tasks:  

- [ ] Develop authentication and authorization layers.  
- [ ] Implement rate limiting and request validation.  
- [ ] Provide API documentation for ease of use.  
- [ ] Monitor API logs for suspicious activities.  

## Metrics for Success:  

- **Security:** 0 security breaches during testing.  
- **Performance:** API response times <500ms for 95% of requests.  
- **Usability:** >90% developer satisfaction with API documentation and ease of use.  

## Outcome:  

- A secure and efficient API that enables seamless data interaction for AI developers.

### System Requirement 5: Logging & Monitoring for Data Integrity  

As a system architect, I want a logging and monitoring system to track data modifications so that I can ensure data integrity and accountability.  

## Assumptions:  

1. AI developers need visibility into data changes for debugging and compliance.  
2. System logs can help detect anomalies or unauthorized modifications.  

## Validation:  

- Analyze logging data to identify trends in data modifications.[1]  
  - **Follow-Up Questions:**  
    - What trends are observed in the logging data?  
    - How are these trends used to improve data integrity?  

- Ensure logs capture key events without affecting system performance.[2]  
  - **Follow-Up Questions:**  
    - What key events are captured in the logs?  
    - How is system performance monitored during logging?  

- Test retrieval of historical logs for audit purposes.  [2]
  - **Follow-Up Questions:**  
    - How often are historical logs retrieved for audits?  
    - What challenges are faced during log retrieval?  

## Preliminary Tasks:  

- [ ] Implement a logging mechanism for all data modifications.  
- [ ] Develop a monitoring dashboard to track key metrics.  
- [ ] Set up alerts for unusual data changes.  
- [ ] Optimize log storage for efficient retrieval.  

## Metrics for Success:  

- **Log Completeness:** 100% of key events captured.  
- **System Performance:** <5% performance overhead due to logging.  
- **Audit Efficiency:** Historical logs retrievable within 2 minutes.  

## Outcome:  

- A robust logging and monitoring system that ensures data transparency and accountability.

### System Requirement 6: Efficient Search & Query Engine for Training Data  

As a system architect, I want an efficient search and query engine so that I can enable AI developers to find relevant training data quickly.  

## Assumptions:  

1. Large datasets require advanced search capabilities for efficient retrieval.  
2. Developers need to filter data based on various criteria.  

## Validation:  

- Measure search response times under different query loads.[1]
  - **Follow-Up Questions:**  
    - What are the current search response times?  
    - How do these times vary under different query loads?  

- Compare search accuracy before and after implementing indexing techniques.[1]  
  - **Follow-Up Questions:**  
    - How accurate are the search results before and after indexing?  
    - What indexing techniques are used?  

- Gather developer feedback on ease of use and relevance of search results.  [2]
  - **Follow-Up Questions:**  
    - How do developers rate the ease of use of the search engine?  
    - How relevant are the search results to their needs?  

## Preliminary Tasks:  

- [ ] Implement full-text search with indexing for fast retrieval.  
- [ ] Develop filtering options based on metadata attributes.  
- [ ] Optimize query performance using caching mechanisms.  
- [ ] Test the system’s ability to handle complex search queries.  

## Metrics for Success:  

- **Search Speed:** Response times <1 second for 95% of queries.  
- **Search Accuracy:** >90% relevance in search results.  
- **Developer Satisfaction:** >85% satisfaction rate with search functionality.  

## Outcome:  

- A high-performance search engine that enables quick and accurate data retrieval.

# Reference:

[1] github.com. (n.d.). Line breaks. docs.github.com. [https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#line-breaks](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#line-breaks)

[2] IBM. (2023). Shedding light on AI bias with real world examples. [https://www.ibm.com/](https://www.ibm.com/). [https://www.ibm.com/think/topics/shedding-light-on-ai-bias-with-real-world-examples](https://www.ibm.com/think/topics/shedding-light-on-ai-bias-with-real-world-examples)

[3] www.reddit.com. (2023). AI-powered web scraper? [https://www.reddit.com/r/ChatGPTPro/comments/18nxnzd/aipowered_web_scraper/](https://www.reddit.com/r/ChatGPTPro/comments/18nxnzd/aipowered_web_scraper/)

[4] www.appian.com/](https://appian.com/). (2024). How Does AI Model Training Work? [https://appian.com/blog/acp/ai/how-does-ai-model-training-work](https://appian.com/blog/acp/ai/how-does-ai-model-training-work)

