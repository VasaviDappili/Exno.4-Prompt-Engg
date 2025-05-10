# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:10-05-2025                                                                           
### REGISTER NUMBER : 212223040030
### Developed by: DAPPILI VASAVI

### Aim:
To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

## Algorithm: 
## 1. Direct Instruction Prompting
## Objective: Guide the chatbot to respond concisely to customer inquiries.
## Prompt Pattern:
## Prompt:

"When a customer asks for the status of their order, reply with:
'Your order is currently being processed and will be delivered by [date].'"
## Use Case:
For quick and clear responses to common queries such as order status, refund confirmation, or operating hours.

## 2. Contextual Prompting
## Objective: Incorporate specific context to provide detailed answers based on the user’s previous interaction.
## Prompt Pattern:
## Prompt:

"If the customer previously mentioned that they haven’t received their order, say:
'I see that you mentioned your order hasn't arrived yet. Let me check the details for you and get back shortly.'"
## Use Case:
Useful for multi-turn conversations where the chatbot must remember and reference earlier parts of the chat to maintain coherence.

## 3. Persona-Based Prompting
## Objective: Design the chatbot to adopt a specific persona, making the interaction more engaging.
## Prompt Pattern:
## Prompt:

"Pretend you are a friendly, helpful customer service representative. Use a conversational tone, such as:
'Hey there! I’m here to help with any questions you might have. Let’s get your issue sorted!'"
## Use Case:
Best for enhancing customer experience by making the bot feel more human-like, on-brand, and approachable.

## 4. Few-Shot Prompting
## Objective: Teach the AI how to respond using a few examples, enabling it to generalize for similar situations.
## Prompt Pattern:
## Prompt:

"Here are some examples of how to handle technical questions:
'My phone isn't charging.' → 'Have you tried using a different cable? If that doesn’t work, it may be an issue with the port.'
'The screen is flickering.' → 'It sounds like a display issue. Have you tried restarting the device?'
Now, respond to: 'My app keeps crashing.'"
## Use Case:
Ideal for training the chatbot on how to respond to less common or varied support requests with appropriate tone and content.

## 5. Chain of Thought Prompting
## Objective: Use a step-by-step reasoning approach for resolving more complex or technical issues.
## Prompt Pattern:
## Prompt:

"When a customer reports their laptop overheating, guide them through the following steps:
Ask if they are using the laptop on a soft surface.
Suggest moving the laptop to a flat, hard surface for better airflow.
Ask if they’ve cleaned the vents recently.
Recommend restarting the device to see if the issue persists.
Now, solve: 'My laptop fan is making a loud noise.'"
## Use Case:
Helpful in tech support scenarios where the problem-solving process involves logical sequencing and troubleshooting.

## 6. Instruction with Constraints
## Objective: Instruct the chatbot to provide assistance while adhering to specific constraints (e.g., response length or tone).
## Prompt Pattern:
## Prompt:

"Respond to order inquiries in no more than 50 words and avoid using technical jargon.
For example: 'Your order is on the way and should arrive by [date]. Feel free to reach out if you need anything else.'"
## Use Case:
Useful when the chatbot must respond within tight UX or brand guidelines—such as character limits, simplicity for non-tech users, or specific voice guidelines.

## 7. Reflective Prompting
## Objective: Ensure that the chatbot reflects the user’s query back to them before providing a response, reducing misunderstandings.
## Prompt Pattern:
## Prompt:

"When a customer asks for help, first reflect their question back to them.
For example, if they ask 'How can I reset my password?' respond with:
'You're asking how to reset your password, correct? Here’s how you can do it.'"
## Use Case:
Best used in sensitive or high-stakes conversations (e.g., billing, account access), where confirming intent avoids errors or miscommunication.

## Algorithm:
## STEP 1: Define the Use Case

Goal: Help users schedule or manage medical appointments.

Target: Patients interacting via a hospital website or mobile app.

## STEP 2: Select Suitable Prompting Techniques

Based on complexity, context sensitivity, and emotional tone.

## STEP 3: Design Prompt Templates

Use appropriate language structure, tone, and sample interactions.

## STEP 4: Implement Prompt-Driven Responses

Feed prompts into a language model to simulate chatbot dialogue.

## STEP 5: Test and Evaluate

Compare outputs from different techniques.

Validate accuracy, tone, and contextual understanding.

## 🧪 PROMPTS & OUTPUT OVERVIEW

## 🔄 Revised Prompting Strategy: Clarification-Based Prompting
## 🔹 Objective:
To improve the chatbot’s accuracy by encouraging it to ask clarifying questions before giving a solution when user queries are vague or ambiguous.

## 🧪 PROMPTS & OUTPUT OVERVIEW
1. Clarification-Based Prompting
Objective: To handle unclear queries by prompting the AI to ask follow-up questions before responding.

## Prompt:

"If a customer says, 'My product isn't working,' ask a clarifying question before attempting to solve the issue. For example:
'I'm sorry to hear that! Could you please tell me which product you're referring to and describe the issue in a bit more detail?'"

## ChatGPT Output:
Response: “I'm sorry you're having trouble. Could you let me know which product you're referring to and what specifically isn't working?”

Behavior: Requests clarification before providing a solution.

## Claude Output:
Response: “Thanks for reaching out! Can you tell me which product you're using and describe the issue you’re facing? That way, I can help more effectively.”

Behavior: Polite and context-seeking before troubleshooting.

| **Platform** | **Clarifying Strategy**      | **Tone**             | **Analysis**                                             |
| ------------ | ---------------------------- | -------------------- | -------------------------------------------------------- |
| **ChatGPT**  | Direct and to the point      | Polite and efficient | Good at quickly identifying ambiguity and resolving it.  |
| **Claude**   | More conversational and warm | Friendly and helpful | Adds a human-like warmth, ideal for customer engagement. |


## Evaluation:
Empathy: Claude provides a warmer, human-like interaction.

Clarity: ChatGPT is more straightforward, making it faster in time-sensitive cases.

Effectiveness: Both prompt the user for details, ensuring better problem-solving.

Usefulness: This prompt type is ideal when users express vague problems.


## 🔄 Revised Prompting Strategy: Scenario-Based Problem Solving Prompt
## 🔹 Objective:
To have the chatbot approach problem-solving by considering all details of a given scenario and offering a customized solution based on the user's context.

## 🧪 PROMPTS & OUTPUT OVERVIEW
2. Scenario-Based Problem Solving Prompt
Objective: Guide the AI in analyzing a scenario and suggesting a solution that fits the user’s needs or problem.

## Prompt:

"A customer reports their internet connection is very slow, but they haven't mentioned if they're using a wired or wireless connection. Your task is to ask the user about their setup and suggest potential solutions based on their response."

## ChatGPT Output:
Response: “Thanks for reaching out! To help you better, could you let me know if you're using a wired or wireless connection? I can provide more specific advice once I know this.”

Behavior: Requests further details before troubleshooting.

## Claude Output:
Response: “I’m sorry to hear that! Could you tell me whether you’re connected to the internet via a wired connection or using Wi-Fi? This will help me narrow down possible solutions for you.”

Behavior: Engages with the customer politely and gathers necessary details for troubleshooting.

| **Platform** | **Problem-Solving Approach** | **Tone**              | **Analysis**                                                                               |
| ------------ | ---------------------------- | --------------------- | ------------------------------------------------------------------------------------------ |
| **ChatGPT**  | Direct and efficient         | Polite and concise    | ChatGPT is quick to seek clarification before offering a solution.                         |
| **Claude**   | Warm and inviting            | Friendly and engaging | Claude takes a slightly more conversational approach, which could enhance user experience. |

## Evaluation:
Effectiveness: Both models focus on gathering the right information before solving the problem.

Tone & Engagement: Claude’s response is warmer, which might help build rapport with customers.

Clarity: ChatGPT is straightforward, making it ideal for faster responses.

## 🔄 Revised Prompting Strategy: Emotional Intelligence Prompt
## 🔹 Objective:
To guide the AI in recognizing and responding to the emotional tone of the user’s message, offering empathy or support to make the interaction more human-like and emotionally engaging.

## 🧪 PROMPTS & OUTPUT OVERVIEW
3. Emotional Intelligence Prompt
Objective: The AI recognizes the emotional tone of a user's query and provides a response that is empathetic or supportive based on the user's feelings.

## Prompt:

"When a customer says, 'I’m so frustrated with my purchase, it’s not working as expected,' your task is to recognize their frustration and respond with empathy, offering help and understanding."

## ChatGPT Output:
Response: “I’m really sorry to hear that you're feeling frustrated. I understand how disappointing it can be when things don’t work as expected. Let me help you resolve this issue quickly.”

## Behavior: Acknowledges the user's frustration and provides support with a solution-oriented approach.

## Claude Output:
Response: “I can definitely understand your frustration—it’s so frustrating when things don’t work the way they should. Let me take a look at your issue and make sure we get it sorted out for you.”

Behavior: Displays empathy and encourages further interaction with a solution-oriented mindset.

| **Platform** | **Emotional Tone Detection** | **Response Style**             | **Analysis**                                                                                                    |
| ------------ | ---------------------------- | ------------------------------ | --------------------------------------------------------------------------------------------------------------- |
| **ChatGPT**  | Recognizes frustration       | Empathetic and problem-solving | ChatGPT effectively shows empathy while quickly moving towards solving the problem.                             |
| **Claude**   | Recognizes frustration       | Compassionate and encouraging  | Claude’s approach is slightly more emotionally supportive, offering reassurance in addition to problem-solving. |


## Evaluation:
Empathy: Claude has a warmer, more encouraging tone that may help build rapport with users.

Effectiveness: Both platforms show empathy, but Claude's response is more emotionally supportive.

Engagement: Both responses encourage further interaction, but Claude’s tone may encourage more positive engagement due to its supportive nature.

## ✅ Summary of Prompt Performance

| Prompt Type                 | Best Performer | Reason                                              |
| --------------------------- | -------------- | --------------------------------------------------- |
| Preceding Question Prompt   | Tie            | Both gave accurate and useful sentiment predictions |
| Comparative Analysis Prompt | Claude         | Offered better insight into tone and language       |
| Experiential Perspective    | Claude         | More emotionally aware and customer-centric         |


## ✅ Conclusion
1.Prompting techniques enhance the chatbot's performance in different scenarios.

2.A mix of instruction-based and persona-based prompting provides both clarity and emotional support in healthcare settings.

3.Chain-of-thought and few-shot prompting are especially effective for multi-step and varied queries.

## Result:
The various types of prompts were executed successfully, guiding the chatbot in resolving customer queries effectively while maintaining a friendly, efficient, and responsive interaction.












