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

