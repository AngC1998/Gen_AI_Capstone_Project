# Gen_AI_Capstone_Project

As a Data Scientist in Healthcare with over two years of industry experience, I’ve learned that a person’s zip code (postal code) plays a crucial role in determining their health status. Where an individual lives can significantly impact their overall health, as local healthcare quality varies across regions. Unfortunately, many people are unaware of the healthcare facilities available in their area or may not know which one is best suited for their specific medical needs. To address this, I developed EmergencyZIP AI, a tool designed to help individuals identify the best medical facilities based on their symptoms or conditions, while considering their zip code as a critical factor in their health status.

## Use Case and Solution Approach
Individuals often seek clarity about the illness or medical condition they may be experiencing and want to know which nearby healthcare facilities can provide the best treatment. EmergencyZIP AI utilizes advanced AI to not only help individuals identify the potential illness or condition they’re facing but also guide them to the most appropriate medical facilities nearby based on zip code.

The system takes zip codes into account, recognizing the importance of location in determining healthcare accessibility and quality.

## Innovation/Novelty
Although the internet provides many resources for finding local healthcare facilities, searching through numerous results can be overwhelming. Moreover, it’s difficult for individuals to accurately diagnose their condition without medical expertise. EmergencyZIP AI solves this by offering personalized and tailored responses, focusing specifically on the individual’s symptoms and their location.

While human doctors are skilled at diagnosing, they may still be influenced by biases or errors. AI, on the other hand, minimizes these biases by considering the patient’s demographic information. However, I acknowledge that human doctors can recognize nuances that AI may miss, as AI is typically trained on generalized data. The goal of EmergencyZIP AI is to make medical information more accessible and less overwhelming for users, while providing individualized insights.

## Process
EmergencyZIP AI operates using Structured Output/JSON Mode/Controlled Generation, Few-Shot Prompting, and Grounding techniques. Here’s how it works:

* JSON Mode: The AI processes the patient’s demographic information and current symptoms, converting it into a structured JSON format, similar to a simplified patient intake form.
* Few-Shot Prompting: The AI generates a request based on the information provided by the JSON form using a few provided examples to maintain consistency and accuracy which is then included in a prompt for the AI asking for the most relevant data to help diagnose the condition. The AI also extracts zipcode from the JSON form using a few provided examples to maintain accuracy to be used to find nearby locations.
* Grounding: Using the provided information, the AI offers the most accurate potential diagnosis for the individual’s symptoms. Then, it uses the zip code to find the nearest and most appropriate medical facilities for treatment. Then, the AI provides payment and insurance plan information for each recommended location.
* Controlled Generation: As the AI is responsible for providing the most accurate and thorough information as possible, we try to keep the temperature (degree of randomness of output) parameter as low as possible while the top-p (the maximum cumulative probability that the model can reach to select tokens as candidates) parameter as high as possible.

## Limitations and Possible Next Steps
While EmergencyZIP AI functions as intended, it is a basic implementation due to time constraints. Some advanced features were not included due to limitations in the development process (e.g., Python input errors). Additionally, grounding-based responses can sometimes be inaccurate, so the AI should not be considered a replacement for professional medical advice. It provides potential diagnoses and recommendations that should be treated as informational rather than authoritative.

Future improvements include:

* Transitioning the AI into an AI Agent using LangGraph.
* Implementing an interactive feature where users input their information, and the AI processes and responds with relevant recommendations.
* Developing a UX/UI interface for a more user-friendly experience.
* Expanding the JSON form to capture additional information, such as address, health history, sexuality, and income.

## Conclusion and Potential Impact
I created EmergencyZIP AI to provide individuals with a more individualized and accessible way to understand their symptoms, find appropriate treatment options, and consider the crucial role of zip codes in determining their health. While the current version is basic due to time constraints, it functions as intended, helping users make informed decisions about their healthcare.

The goal of this AI is to empower individuals to take charge of their health by providing them with easy access to healthcare resources. Ultimately, I hope EmergencyZIP AI will contribute to improving health outcomes in various regions, one zip code at a time. By helping individuals become more health-conscious and informed, this tool has the potential to make a significant impact on healthcare access and overall well-being.

Medium Blog Post: https://medium.com/@angela.cao.98/emergencyzip-ai-00b11d711e26

YouTube Video: https://youtu.be/aYR06Dws1Xc
