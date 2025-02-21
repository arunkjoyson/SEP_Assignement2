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
### Q) Analysis of current 2 requirements: 

### Requirement 1: Categorized Training Questions & Answers

As an AI developer, I want training questions to be categorized separately from answers so that I can ensure self-affirmation.

## Assumption:

- Developers benefit from self-affirmation when questions and answers are separated.

- Categorization improves retrieval, filtering, and dataset usability.

## Validation:

- Ask developers how often they struggle with mixed question-answer data when using training datasets.

- Do you think determining whether categorization improves searchability and organization in AI training?

  - **Follow-Up Questions:**

    - What methods were tried before to organize?

    - What are the common categories you think are good?

- Do you actively use datasets with separate questions and answers to measure self-affirmation impact?

- Do you think categorization is enough to fix this issue?

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

- Unbalanced training data negatively affects AI model performance.  
- Biases exist in web-scraped data and need mitigation.  

## Validation:  

- Do analysis of scraped training data to check for common biases (e.g., gender, racial, political biases).  
  - **Follow-Up Questions:**  
    - What methods are currently used to detect biases in the training data?  
    - How frequently are biases identified in the current datasets?  

- Compare AI performance metrics before and after applying bias mitigation techniques.  
  - **Follow-Up Questions:**  
    - What specific performance metrics are used to evaluate AI models?  
    - How significant is the performance improvement after bias mitigation?  

- Gather feedback from developers on whether biased datasets have affected their previous models.  
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

- AI developers collect training data through web scraping.  
- Web scraping is the most efficient method to gather large-scale training data.  
- Publicly available data can be used without legal restrictions.  

## Validation:  

- How do you collect training data?  
- Ask whether the current web scraping process is manual or semi-automated.  
  - **Follow-Up Questions:**  
    - How is the current web scraping process managed? Is it fully manual, semi-automated, or automated?  
    - What are the main challenges faced with the current process?  

- Check if existing AI training workflows depend on external scraping tools.  
  - **Follow-Up Questions:**  
    - Are there any specific external scraping tools currently in use? If so, which ones?  
    - How do these tools impact the overall AI training workflow?  

- Confirm compliance with data collection regulations (e.g., robots.txt, legal policies).  
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

- Not all data sources are equally valuable, and developers need filtering options.  
- Scraping frequency needs to be adjustable based on data availability and project needs.  

## Validation:  

- Gather feedback from developers on the most commonly needed filtering parameters.  
  - **Follow-Up Questions:**  
    - What filtering parameters do you find most useful in your current workflow?  
    - How often do you need to adjust scraping parameters?  

- Determine whether frequent scraping causes redundant or unnecessary data collection.  
  - **Follow-Up Questions:**  
    - Have you experienced issues with redundant data collection? If so, how often?  
    - How do you currently manage redundant or unnecessary data?  

- Assess if parameter customization improves data quality and reduces preprocessing effort.  
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

- Automated scraping may introduce errors, irrelevant content, or biased data.  
- Manual review is necessary to refine training datasets.  

## Validation:  

- Analyze how often developers manually correct training data in existing workflows.  
  - **Follow-Up Questions:**  
    - How frequently do you manually review and correct training data?  
    - What types of errors or issues do you commonly encounter during manual review?  

- Compare model performance before and after manual data curation.  
  - **Follow-Up Questions:**  
    - How does manual data curation impact your model's performance?  
    - Can you provide examples of improvements seen after manual review?  

- Determine if automated pre-filtering can reduce the need for manual review.  
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

- Developers prefer seamless integration with existing AI tools.  
- Manually exporting/importing data slows down the workflow.  

## Validation:  

- Identify the most commonly used AI training platforms requiring integration.  
  - **Follow-Up Questions:**  
    - Which AI training platforms do you currently use?  
    - What integration features are most important to you?  

- Ensure API usability with different programming languages and frameworks.  
  - **Follow-Up Questions:**  
    - What programming languages and frameworks do you use for AI development?  
    - Have you encountered any issues with API usability in the past?  

- Test API speed, security, and reliability under heavy data loads.  
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

- Training data modifications impact AI model performance and need traceability.  
- Developers need to track changes to debug and refine datasets.  

## Validation:  

- Identify if developers currently struggle with tracking data modifications.  
  - **Follow-Up Questions:**  
    - How do you currently track modifications to your training data?  
    - What challenges do you face with the current tracking methods?  

- Determine if auditing improves dataset consistency and debugging.  
  - **Follow-Up Questions:**  
    - How has auditing impacted your ability to maintain dataset consistency?  
    - Can you provide examples of how auditing has helped in debugging issues?  

- Test the impact of detailed logs on system performance and usability.  
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

- Large datasets become unmanageable without proper filtering tools.  
- Developers need advanced search options for efficient data retrieval.  

## Validation:  

- Analyze how developers currently search for training data.  
  - **Follow-Up Questions:**  
    - How do you currently search for and retrieve training data?  
    - What challenges do you face with the current search and filtering methods?  

- Determine if search and filtering improve dataset usability and processing speed.  
  - **Follow-Up Questions:**  
    - How has the implementation of search and filtering tools impacted your workflow?  
    - Can you provide examples of improvements in data retrieval efficiency?  

- Test the impact of different indexing methods on performance.  
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

