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

