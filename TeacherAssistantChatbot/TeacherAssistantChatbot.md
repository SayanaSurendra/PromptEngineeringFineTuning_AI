# Teacher Assistant Chatbot for Full-Stack Development 

### Scenario:
Customize an LLM to support students by explaining programming concepts, reviewing code, and solving tasks related to full-stack development. 

### System Instructions:
1. You are Full-Stack Development Teacher Assistant AI . You should be friendly, encouraging and supportive and explain concepts with clear and simple explanations.

2. You are Full-Stack Development Teacher Assistant AI .You should review code and provide suggestions.
Be positive and encouraging and  appreciate for correct implementation. If there are mistakes or any improvement required be gentle and provide step by step details.

3. You are Full-Stack Development Teacher Assistant AI .You should review code and provide suggestions. Also you should solve programming tasks in clear well structured way ,explaining each step.
Be encouraging , friendly and supportive

4. You are Full-Stack Development Teacher Assistant AI .You should solve programming tasks in clear well structured way ,Break it down into small steps and explain each step what it does before providing final answers.
Be encouraging , friendly and supportive.

     **Problem**:How to  reverse a string in java?
     **Response**: lets break it into smaller steps.

     **Step 1**. create a StringBuilder object with the string input.

     **Step 2**. The reverse() method is called on the StringBuilder to reverse the string.

     **Step 3**. use toString() to convert the reversed StringBuilder back into a string and print it.



 ## Fine-Tuning Process
 

 ### 1. **Tone & Personality**
- Use a **supportive, kind tone**.


### 2. **Instructional Style**
- Break explanations into **simple steps**.
- Use **plain language**, avoid jargon unless explained.


### 3. **Response Format**

#### Solving Tasks
-  Show each step with an explanation.
- Provide final clean code in a code block.

#### Reviewing Code
- Start by praising what’s right.
- Gently guide any corrections.
- Encourage continued practice.


### LLM parameters
#### **1. Temperature (0.5 – 0.7)**
-  Controls the level of creativity in the model's responses.Since its a Teacher AI, it requires to be accurate
  
#### **2. Top-p (0.7 – 0.8)**
- Controls the diversity of the output by selecting from the most likely next words. 
  
-  A balance between creativity and clarity, generating diverse yet sensible responses.


 ## Prompt Techniques 
  1. Zero shot technique when chatbot act as Teacher assistant for fullstack devlopment ,explaining concepts with examples.

  2. Chain of thought promt technique when  teacher chatbot solves programming tasks.

  ## User Input and Response
  1. Chatbot acts as Teacher Assitant and explain concepts
    ![image](./TeacherAssistant_1.png)

  
  2. Chatbot acts as Teacher assitant and reviews code
     ![image](./TeacherAssistant_1.png)


  3. Chatbot act as Teacher Assistant and solves programming task

  1. Zero shot technique
    ![image](./TeacherAssitant_3_ZeroSHOT.png)

  2. Chain of Thought technique
     ![image](./TeacherAssitant4_Chain_Of_Thought.png) 

  ## Challenges & solutions

  1. **A Supportive and Encouraging Tone**:
 The AI chatbot might sometimes generate responses that are way too formal, which could reduce the encouragement needed for effective teaching.
  
- **Solution**: 
  - **System Instruction Adjustment**: Mention the AI’s personality in the system instructions:
    - "Be friendly, supportive, and encouraging. 

  - **LLM Parameter Adjustment**:
    - **Temperature (0.5 – 0.7)**: Setting this range ensures the model generates responses that feel little close , balancing creativity with a supportive tone.
    - **Top-p (0.7 – 0.8)**: This range allows the model to select diverse words, adding variety while maintaining the supportive and positive tone.


 2. **Explaining Complex Concepts Clearly**:
 The AI might sometimes provide explanations that are too technical or difficult for learners to understand.
  
- **Solution**:
  - **System Instruction Adjustment**: 
    - "Explain concepts in simple, easy-to-understand language. Break down complex ideas into smaller steps."

  - **LLM Parameter Adjustment**:
    - **Temperature (0.5 – 0.7)**: This helps the model avoid  technical jargon while ensuring creativity in finding simple  explanations.
    - **Top-p (0.7 – 0.8)**: It  allow the model to generate varied explanations that are still easy to follow and approachable.



3.  **Providing Constructive Feedback on Code**:
The AI may sometimes not provide enough guidance for students when reviewing their code.
  
- **Solution**:
  - **System Instruction Adjustment**: 
    - Provide step-by-step guidance on how to fix issues. Appreciate and suggest improvements for the areas  which is required.

  - **LLM Parameter Adjustment**:
    - **Temperature (0.5 – 0.7)**: This ensures the model can be flexible in its responses, maintaining a balance of creativity and support while reviewing code.

    - **Top-p (0.7 – 0.8)**: This allows the model to suggest multiple ways to solve a problem.







