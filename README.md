# Exno.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques
### DATE:                                                                            
### REGISTER NUMBER : 212223040030
### Developed by: DAPPILI VASAVI

### Aim:
To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

## Algorithm: 

## 1. Direct Instruction Prompts
### Objective: Guide the chatbot to respond concisely to customer inquiries.

### Prompt Pattern:

### Prompt:
"When a customer asks for the status of their order, reply with: 'Your order is currently being processed and will be delivered by [date].'"

## 2. Contextual Prompting

Objective: Incorporate specific context to provide detailed answers based on the user’s previous interaction.

### Prompt Pattern:

### Prompt: 
"If the customer previously mentioned that they haven’t received their order, say, 'I see that you mentioned your order hasn't arrived yet. Let me check the details for you and get back shortly.'"

## 3. Persona-Based Prompting

### Objective: Design the chatbot to adopt a specific persona, making the interaction more engaging.

### Prompt Pattern:

### Prompt: 
"Pretend you are a friendly, helpful customer service representative. Use a conversational tone, such as 'Hey there! I’m here to help with any questions you might have. Let’s get your issue sorted!'"

## 4. Few-Shot Prompting

### Objective: Teach the AI how to respond using a few examples, enabling it to generalize for similar situations.

### Prompt Pattern:

### Prompt: 
"Here are some examples of how to handle technical questions:

'My phone isn't charging.' → 'Have you tried using a different cable? If that doesn’t work, it may be an issue with the port.'
'The screen is flickering.' → 'It sounds like a display issue. Have you tried restarting the device?'

Now, respond to: 'My app keeps crashing.'"

## 5. Chain of Thought Prompting

### Objective: Use a step-by-step reasoning approach for resolving more complex or technical issues.

### Prompt Pattern:

### Prompt: "When a customer reports their laptop overheating, guide them through the following steps:

Ask if they are using the laptop on a soft surface.

Suggest moving the laptop to a flat, hard surface for better airflow.

Ask if they’ve cleaned the vents recently.

Recommend restarting the device to see if the issue persists.

Now, solve: 'My laptop fan is making a loud noise.'"

## 6. Instruction with Constraints

### Objective: Instruct the chatbot to provide assistance while adhering to specific constraints (e.g., response length or tone).

### Prompt Pattern:

### Prompt:
"Respond to order inquiries in no more than 50 words and avoid using technical jargon. For example, 'Your order is on the way and should arrive by [date]. Feel free to reach out if you need anything else.'"

## 7. Reflective Prompting

### Objective: Ensure that the chatbot reflects the user’s query back to them before providing a response, reducing misunderstandings.

### Prompt Pattern:

### Prompt:
"When a customer asks for help, first reflect their question back to them. For example, if they ask 'How can I reset my password?' respond with 'You're asking how to reset your password, correct? Here’s how you can do it.'"

Result: The various types of Prompts are executed successfully.

## 📚 Use Case

**Social Media Posts:**  
The system is designed to tailor product recommendations based on user preferences such as past `posts, browsing history, and selected interests.
For each prompt type, the AI tools (ChatGPT and Claude) are asked to analyze a social media post and predict sentiment, engagement potential, and offer insights into tone and language used.

---

## ⚙️ ALGORITHM

### Step 1: Define Use Case
We are analyzing a set of social media posts to determine public sentiment, engagement levels, and actionable insights. The goal is to evaluate the effectiveness of each prompting technique on two different AI platforms: **ChatGPT** and **Claude**.

### Step 2: Define Prompting Techniques
1. **Preceding Question Prompting:** Use a question that references the context of the post or its content for analysis.
2. **Comparative Analysis Prompt:** Ask the model to compare the current post with others or with a specific benchmark.
3. **Experiential Perspective Prompt:** Request the model to analyze the post as if it's a real-life scenario or with a human perspective.

### Step 3: Submit Prompts to AI Tools
Each prompt will be tested on both **ChatGPT** and **Claude** to observe how they handle different contexts and sentiment analysis.

### Step 4: Collect Outputs
Record the outputs from both platforms for each of the three prompts.

### Step 5: Analyze Outputs
Evaluate the output for:

- Accuracy of sentiment analysis
- Relevance of the response
- Insightfulness of the analysis
- How well the AI models handle the type of prompt provided

---

## 🧪 PROMPTS & OUTPUT OVERVIEW

### 1. Preceding Question Prompting

- **Objective**: To analyze sentiment and predict engagement based on context from the preceding questions.
 
**Prompt:**
> "Given the following social media post, can you assess the public sentiment and predict the level of engagement? 
> 'Just launched our new eco-friendly product line! Super excited to make a difference. #SustainableLiving #EcoFriendlyProducts'"

- **ChatGPT Output:**
  - Sentiment: Positive
  - Engagement Prediction: High, due to the excitement around sustainability.
  - Reasoning: The post conveys enthusiasm, which often correlates with higher engagement.

- **Claude Output:**
  - Sentiment: Positive
  - Engagement Prediction: Likely to generate significant engagement due to popular hashtags and a focus on sustainability.
  - Reasoning: Focus on eco-friendliness and the use of trending hashtags suggests higher engagement.


| **Platform**   | **Sentiment** | **Engagement Prediction** | **Analysis** |
|----------------|---------------|---------------------------|--------------|
| **ChatGPT**    | Positive      | High                      | ChatGPT provided an accurate sentiment analysis and correctly predicted engagement based on sustainability themes. |
| **Claude**     | Positive      | High                      | Claude mirrored ChatGPT’s result with a similar conclusion, providing accurate sentiment and a high engagement prediction. |

#### Evaluation:
- **Accuracy**: Both platforms performed well, identifying the correct sentiment and engagement.
- **Coherence**: Both outputs aligned logically with the context of the post.
- **Simplicity**: The responses were clear and easy to understand.
- **Speed**: Both platforms performed the analysis quickly.
  
---

### 2. Comparative Analysis Prompt

- **Objective**: To compare a given post with a typical marketing post, highlighting differences in tone, language, and engagement prediction.
  
**Prompt:**
> "Compare the following social media post with a typical marketing campaign post. How does it differ in terms of tone, language, and engagement potential?
> 'We're so happy to announce the launch of our latest product line—crafted with care and designed for you! #NewArrival #Fashion'"

- **ChatGPT Output:**
  - Tone Comparison: The tone of this post is warmer and more customer-centric compared to a typical product-focused post.
  - Language: More personal language is used compared to the impersonal, sales-driven tone of standard marketing posts.
  - Engagement: Likely moderate engagement due to its neutral tone.

- **Claude Output:**
  - Tone Comparison: The tone is soft and personal, different from the more aggressive tone typically found in traditional marketing.
  - Language: The language is customer-friendly, inviting, and informal, in contrast to more formal marketing language.
  - Engagement: Likely moderate, as the tone may attract customers but lacks urgency or excitement.


| **Platform**   | **Tone Comparison**  | **Language**  | **Engagement Prediction** | **Analysis** |
|----------------|----------------------|---------------|---------------------------|--------------|
| **ChatGPT**    | More customer-centric| Softer tone   | Moderate                  | ChatGPT compared the tone accurately but lacked deep insights into how the language affects engagement. |
| **Claude**     | Personal, softer     | Informal, customer-friendly | Moderate                  | Claude provided a more nuanced comparison, focusing on subtle differences between marketing and customer-friendly language. |

#### Evaluation:
- **Insightfulness**: Claude’s response was more detailed and nuanced in analyzing tone, language, and engagement.
- **Tone & Language**: Both platforms accurately identified differences, but Claude provided deeper insight.
- **Engagement Potential**: Both predicted moderate engagement but lacked urgency, which could impact engagement.
- **Speed**: Both platforms quickly generated the analysis.

---

### 3. Experiential Perspective Prompt

- **Objective**: To analyze the post from a customer’s perspective and predict engagement based on emotional tone and content.

**Prompt:**
> "Imagine you are a customer reading this post. How would you feel, and would you be inclined to engage with the content? 
> 'We are thrilled to announce our partnership with local artisans to bring you unique, handcrafted items that reflect our values of sustainability.'"

- **ChatGPT Output:**
  - Emotional Reaction: Positive, feeling of excitement about supporting local artisans and sustainability.
  - Engagement: High, likely to inspire customers to comment and share.
  - Reasoning: The post conveys a sense of community, sustainability, and exclusivity.

- **Claude Output:**
  - Emotional Reaction: Intrigued and inspired, especially by the focus on sustainability and local artisans.
  - Engagement: High, would likely generate positive interaction due to its human-centric message.
  - Reasoning: Engages on a deeper level with a community-driven message.



| **Platform**   | **Emotional Reaction** | **Engagement Insight** | **Analysis** |
|----------------|------------------------|------------------------|--------------|
| **ChatGPT**    | Positive, excited      | High                   | ChatGPT captured the emotional tone well but was less insightful in terms of emotional connection. |
| **Claude**     | Intrigued, inspired    | High                   | Claude provided a more empathetic and emotional response, understanding deeper feelings and engagement drivers. |

#### Evaluation:
- **Empathy**: Claude demonstrated stronger emotional insight, connecting more deeply with the post’s emotional tone.
- **Engagement Insight**: Both platforms predicted high engagement but Claude gave a more emotionally grounded prediction.
- **Relevance**: Claude’s output was more aligned with human emotions and engagement drivers.
- **Speed**: Both responses were quick.
---

## ✅ RESULT: Prompt Performance Summary

| Prompt Type                    | Best Performing Platform | Summary of Findings                                                    |
|---------------------------------|--------------------------|-------------------------------------------------------------------------|
| **Preceding Question Prompting** | Tie (ChatGPT & Claude)    | Both platforms provided strong sentiment analysis with similar engagement predictions. |
| **Comparative Analysis Prompt**  | ChatGPT                   | Better at highlighting the tone differences and provided a more detailed analysis of engagement potential. |
| **Experiential Perspective Prompt** | Claude                    | More human-centric and emotionally engaging responses, providing a stronger insight into customer reactions. |

---

## 🔍 INSIGHTS

- **ChatGPT** was better at analyzing and comparing posts in terms of tone and language.
- **Claude** provided more insightful emotional and engagement predictions, particularly for the experiential prompt.
- **Preceding Question Prompting** showed that both platforms could handle this straightforward task equally well.
- **Comparative Analysis Prompt** and **Experiential Perspective Prompt** yielded nuanced responses, with **Claude** excelling in the latter for human perspective.

---

## 📌 CONCLUSION

- **Preceding Question Prompting** was effective for both **ChatGPT** and **Claude**, producing clear and accurate responses.
- **Comparative Analysis Prompt** showed that **Claude** was better at understanding subtle differences in tone, language, and engagement potential.
- **Experiential Perspective Prompt** demonstrated that **Claude** had a deeper emotional understanding of the post and provided more insightful engagement predictions.

---

## Result:
The various types of prompts were executed successfully, guiding the chatbot in resolving customer queries effectively while maintaining a friendly, efficient, and responsive interaction.

---
