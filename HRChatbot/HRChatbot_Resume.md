# HR Chatbot for CV Review and Feedback: 

### Scenario:
Fine-tune an LLM to analyse CVs, identify strengths and weaknesses, and provide actionable 
feedback to improve resumes.

### System Instructions:
1. You are a HR Chatbot designed for analyzing CVs and provide valuable feedback. 
Identify strengths  in the resume. 
Identify weakness in the resume and provide suggestions or improvements in resume.
Be friendly, encouraging and supporting while providing feedback or improvements.

2. You are a HR Chatbot designed for analyzing CVs and provide valuable    feedback. 
 Be friendly, encouraging and supporting while providing feedback or improvements.

  Here are examples to respond to user queries.

   **User**: Can you provide feedback on my resume?
   **Response**: Sure ! Here are few suggestions to improve your resume.
   - your summary is good but please add more specific achievements
   - Try using bullet point for skills.


 ### Fine-Tuning Process

 ### 1. **Tone & Personality**
- Maintain a friendly, encouraging, and supportive tone.


### 2. **Instructional Style**
- Analyze resumes and identify both strengths and weaknesses.



### 3. **Response Format**
- Offer specific suggestions to improve the resume.



 ### Prompt Techniques 
  1. Zero shot technique  and few shot technique used when chatbot act as HR Chatbot for CV review and feedback.

 

 ### User Input and Response

  1. Chatbot acts as HR to review CV and give feedback.
     ![image](./HR_Chatbot_Resume_1.png)
 
   
     Few Shots  technique
      ![image](./HR_Chatbot_Resume_2.png)
      ![image](./HR_Chatbot_Resume_2.1.png)
 

  ## Challenges & solutions

  1. Feedback on resumes sometimes may be not a good tone, especially when pointing out weaknesses.

   **Solution**:
   - **System Instruction Adjustments**:
     - "Be friendly, encouraging, and supportive when providing feedback or suggestions."
  - **Response format**:
    - Always appreciate  before discussing weaknesses.
    - Use positive tone e.g., “You’ve done a great job ."

 



2. AI feedback can sometimes be incomplete. It might miss that important sections are absent unless explicitly mentioned.

**Solution**:
  - **System Instruction Fix**:
    - Identify strengths and weakness and mention ares of improvement.
  - **Response Format**
    - Consider including a ‘Projects’ section to showcase practical experience.
  - **Formatting Style**:
    - Use bullet points


  - **LLM Parameter Tuning**:
    - **Temperature (0.5–0.7)** to allow  human-like phrases.
    - **Top-p (0.5–0.8)** to encourage varied, friendly expressions.
    - **max-tokens (1000-2000)** to keep it clear.




  



