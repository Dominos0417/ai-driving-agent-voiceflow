# AI Driving License Assistant 

## About the Project
This project is an interactive Conversational AI agent designed to support candidates preparing for the Category B driving license theoretical exam. The system focuses on natural language interaction, user accessibility, and end-to-end automation of the educational process. 

## Tech Stack
* **Conversational Platform:** [Voiceflow](https://www.voiceflow.com/)
* **Logic & Scripting:** JavaScript
* **Integrations:** REST API (Weather/Context data fetching)
* **Automation:** Make.com (formerly Integromat) for automated email reporting
* **System Design:** StarUML (Flowcharts), Figma (Prototyping)

## Key Features
- **Interactive Exam Simulation:** Dynamic test generation and real-time score calculation handled by custom JavaScript logic embedded within the flow.
- **Contextual Knowledge Base:** AI-assisted responses to user queries regarding traffic rules, road signs, and exam procedures.
- **Automated Result Reporting:** Upon completing a mock exam, the system triggers a Make.com webhook via REST API to automatically generate and send a detailed performance summary to the user's email.
- **Dynamic Context:** Integration with external weather APIs to provide users with situational awareness regarding road conditions.

## System Architecture & Visuals
*(Wklej tutaj 2-3 zrzuty ekranu pokazujące skomplikowanie logiki w Voiceflow oraz przykładową rozmowę z botem)*
![Conversation Flowchart](path/to/voiceflow_canvas_screenshot.png)
![Chat Interface Example](path/to/chat_interaction_screenshot.png)

Detailed system architecture, user personas, and flowcharts can be found in the `documentation/` folder.

## How to Run and Test
1. Create a free account on [Voiceflow](https://www.voiceflow.com/).
2. Create a new "Chat" project.
3. Select the **Import** option and upload the `Agent_Prawo_Jazdy.vf` file included in this repository.
4. *(Optional)* To enable the email reporting feature, configure a webhook scenario in Make.com and update the API endpoint within the Voiceflow API block.
5. Click **Run** or **Test** in the Voiceflow canvas to interact with the agent.

## Future Improvements
- Integration with external video APIs to present multimedia questions (similar to the real state exam).
- Expansion of the LLM context window to support multi-language interactions for foreigners taking the exam.