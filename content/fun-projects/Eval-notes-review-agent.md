## Use Case Title
Eval Notes Review Agent: Turning Manual Insights into Actionable Intelligence

## Problem to Solve
Manual evaluations - where humans capture notes to provide feedback on an LLM response -  are necessary to ensure quality, accuracy, and user experience when testing AI systems. But reviewing these notes to identify key issues across the board can be time-consuming and waste valuable resources.  This is a great use case where AI can do the work for you and save valuable time. 

## Solution
Introducing "Eval Notes Review Agent" - this agent was created in ChatGPT. I simply asked it to identify open codes from written  notes and categorize them into axial codes. I also instructed it to create a structured format and generate a summary table of axiom codes with total number of occurrences. Lastly, I asked it to generate a visualization to easily capture the end user attention. The agent can take either a csv/Excel sheet or plain text as an input and does the job for you. The agent can be leveraged for an AI manual evaluations and not limited to just chatbots.

## Demo summary
The Eval Notes Review Agent is an AI tool designed to streamline the manual evaluation process for AI products, specifically a large language model-based enrollment chatbot. The motivation behind creating the agent: as the team approached the evaluation phase of the chatbot project, they needed an efficient way to analyze and categorize feedback from human evaluators. Traditionally, this process involved manually reviewing chatbot responses, identifying errors, and documenting observations referred to as "open codes" in qualitative research.

To enhance this process, I introduced the concepts of open codes (individual observations or issues) and axial codes (broader categories that group related issues). The team was instructed to interact with the chatbot, record their questions and the chatbot responses, and note the most obvious mistakes. These notes were then collected and prepared for analysis.

The Eval Notes Review Agent was developed to automate the review of these notes. It can ingest plain text, CSV, or Excel files containing evaluator feedback. 

To quickly demo, I copied all the collected notes into the agent and requested it to identify themes. The agent processed the data, extracted open codes, and then grouped them into axial codes, effectively categorizing the types of issues found in the chatbots responses.

The agent also generated a summary table showing the frequency of each axial code, helping the team prioritize which issues to address first. Additionally, a heat map visualization was produced to provide a clear overview of the most critical problem areas. The demo revealed that the most common issues were related to tone and conversational style, followed by link and source quality, and then accuracy and content reliability.

The Eval Notes Review Agent offers a fast, scalable solution for reviewing evaluator notes and identifying key areas for improvement, enabling the team to focus their efforts where they are most needed. 

## Impact
I used it to quickly identify key themes from the notes captured during the first evaluation of the Enrollment chatbot, and it easily saved 30 mins of my time. In the first week alone, I had 64 notes captured just from 4 evaluators. So even if this was doable, imagine bringing in another 20-30 evaluators and reviewing their notes manually to identify issues? The agent also generated frequency counts and highlighted the most common error patterns, so teams know exactly which problems to tackle first without combing through hundreds of notes. In short, this agent resulted in time and cost savings and helped in  quickly indentifying key issues to address.

## Test this agent
https://chatgpt.com/g/g-692095523848819185f006677804d3b5-eval-notes-review-agent





