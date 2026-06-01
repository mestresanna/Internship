---
layout: logbook
title: Logbook
---

# Internship Blog

## Anna Mestres

This daily logbook documents my internship experience at [Lanek](https://www.lanek.cl/) in Chile. It is intended to provide a concise record of my day-to-day activities, progress, and learning throughout the internship period. Each entry summarizes the tasks I have completed, any challenges or issues encountered, and the approaches I used to resolve them.

The purpose of this logbook is to track my professional development, reflect on practical experiences, and maintain a structured overview of my contributions within the organization. It will also serve as supporting documentation for my internship requirements and final evaluation.

---

# Week 1

<h2 id="day1">Day 1 - 30/03</h2>

The internship began with a welcome meeting at 11:00 AM, where I was introduced to the office, team members, workflows, and the current tech stack. I was also given access to the company’s GitHub repositories and communication tools, including the different teams I will collaborate with.

I met with Lucas (Software Engineer) to discuss the technical scope of my project. We refined the objectives to better align with the broader system. Afterwards, I conducted initial research and redefined the project scope, focusing on developing a specialized LLM with a RAG pipeline for clinical data in Spanish, including guardrails and simulated patient testing.

<h2 id="day2">Day 2 - 31/03</h2>

I continued researching the project and had a meeting with Johannes (Head of Technology) to review ideas and direction. Based on this discussion, we decided to start with a minimal viable prototype (MVP) to quickly validate approaches.

I implemented a basic RAG pipeline using synthetic data to test whether the model retrieves information correctly without hallucinating. I also attempted to integrate an interface using OpenWebUI, where I encountered several technical issues.

<h2 id="day3">Day 3 - 01/04</h2>

Today I resolved the issues with the interface, and the MVP is now functional. After validating this initial approach, I started developing the foundations of the actual project with a more structured setup, connected to the company’s GitHub.

I also continued researching suitable technologies for our use case. In the afternoon, I attended a meeting at 16:00 to receive updates on the client requirements from UC Christus, to ensure that my work aligns with the larger project of the company.

<h2 id="day4">Day 4 - 02/04</h2>
Today I was introduced to the lab facilities and the ongoing work being carried out there, as well as to the healthcare department collaborating with the lab. I also had the opportunity to assist in some experiments, which provided practical insight into their processes.

Additionally, I attended my first meeting with the project coach based in Belgium via Microsoft Teams. During the day, I was also introduced to new methodologies and technologies relevant to the project.

<h2 id="day5">Day 5 - 03/04</h2>
Today I received the full set of documentation related to the larger project that my work will contribute to. I focused on understanding the overall scope and structure of the project, identifying key components and objectives.

I also conducted research on technologies and tools that could support development at a larger scale, while noting down technical questions for further clarification.

---

# Week 2

<h2 id="day6">Day 6 - 20/04</h2>
After the Easter holidays, I resumed work by focusing on the system architecture of the overall project. Using draw.io, I created two initial diagrams: a detailed version outlining the technical components, and a more general one illustrating the core functionality of the application.

These drafts will serve as a foundation for further refinement.

<h2 id="day7">Day 7 - 21/04</h2>
Today I continued improving the system architecture diagrams, refining both their structure and level of detail. I also carried out additional research on relevant technologies to better support design decisions.

In parallel, I participated in discussions to better define the scope of my project and how it integrates within the broader system.

<h2 id="day8">Day 8 - 22/04</h2>
Today we held several meetings to define the scope of the MVP for the project I will be developing. The definition is still in progress and is expected to be finalized tomorrow after additional discussions with members of the development team.

In parallel, I worked on creating a synthetic dataset to simulate hospital data, as we determined that obtaining real data from the client within the available timeframe would not be feasible. This dataset will be used for initial development and testing.

The next step will be to integrate this simulated data with the RAG prototype developed last week.

<h2 id="day9">Day 9 - 23/04</h2>
Today I focused on rewriting the documentation for the MVP and refining the overall planning based on the latest decisions. I also began working on integrating the database into the system.

In addition, I improved parts of the synthetic dataset to make it more robust and realistic, ensuring better performance and reliability of the RAG pipeline.

<h2 id="day10">Day 10 - 24/04</h2>

Today I completed the integration of the database with the RAG pipeline and began testing it through the interface using OpenWebUI to ensure compatibility.

During testing, I encountered some challenges related to converting database content into a format that is easily interpretable by the LLM. Addressing these issues is necessary to improve the readability and overall performance of the system.

---

# Week 3

<h2 id="day11">Day 11 - 27/04</h2>

Today I focused on thoroughly testing the RAG pipeline to identify potential issues. While the overall workflow is functional, it still lacks a more robust implementation.

I began addressing this by improving the database structure to make it more realistic. I also fixed several bugs related to the database and its automatic generation process.

<h2 id="day12">Day 12 - 28/04</h2>

In the morning, I had a meeting with my tutor to review progress. Afterwards, I continued working on the RAG pipeline, improving the document chunking strategy to enhance retrieval quality.

I developed initial test cases and began implementing the query-response functionality as part of the system.

<h2 id="day13">Day 13 - 29/04</h2>

Today I continued developing the query-response functionality. During this process, I identified issues in the database related to semantic inconsistencies between tables.

I resolved these issues and created updated diagrams along with detailed documentation describing each table, ensuring better clarity and maintainability of the system.

<h2 id="day14">Day 14 - 30/04</h2>

I completed and tested the query-response functionality, which is now working correctly. However, the RAG pipeline still requires improvements, particularly in the use of filters and the retrieval process, which remains relatively basic.

I started refining the retriever and context generation to improve the accuracy of responses. The next steps will include further optimization and implementing latency control mechanisms.

<h2 id="day15">Day 15 - 01/05</h2>

Festivity

---

# Week 4

<h2 id="day16">Day 16 - 04/05</h2>
I refactored the RAG pipeline into a clean, modular architecture separating retrieval, context building, filtering, and reranking into dedicated services. On top of that, I introduced a cohort-based scoring system that ranks similar patients using weighted signals (diagnosis, recency, severity, and semantic similarity) to generate aggregated clinical evidence from historical cases.

<h2 id="day17">Day 17 - 05/05</h2>
Today I tested all the outputs from the work completed the previous day. I also switched to testing the API directly through the terminal to simplify debugging and validation.

In addition, I improved the cohort implementation so the LLM can generate more coherent and contextually accurate responses.

<h2 id="day18">Day 18 - 06/05</h2>
Today I continued improving the RAG responses by refining the cohort implementation. During testing, I discovered a bug in the dataset related to the AI alert system.

After fixing the issue, the overall quality of the responses and the reasoning process of the RAG improved significantly.

<h2 id="day19">Day 19 - 07/05</h2>
Today I started working on the event-driven system using RabbitMQ deployed as a container.

I researched the best approach for integrating events into the current architecture, as the ingestion pipeline was still being triggered manually and reprocessing all chunks each time. I realized that the codebase required refactoring and that additional metadata needed to be introduced for the chunks in order to support selective updates instead of rebuilding the entire dataset.

<h2 id="day20">Day 20 - 08/05</h2>
Today I refactored part of the codebase to introduce a more scalable structure using a hexagonal architecture approach, improving maintainability and future extensibility.

To support the new event-driven workflow, I also redesigned the chunking strategy so that only specific sections of the vector database need to be updated instead of rebuilding the entire Vector DB after each change.

---

# Week 5

<h2 id="day21">Day 21 - 11/05</h2>
Today I worked on implementing event-based updates for diagnostics using RabbitMQ as the communication bus between services. I also created repository layers connected directly to the database API in order to manage and synchronize updates more efficiently.

<h2 id="day22">Day 22 - 12/05</h2>
I focused on debugging and resolving issues introduced during the recent refactoring process. Most of the work was related to ensuring the correct ingestion of data from the main database into the vector database, as well as stabilizing the event injection workflow.

<h2 id="day23">Day 23 - 13/05</h2>
I fixed several inconsistencies related to naming conventions across the project. In addition, I continued debugging the quality of the RAG responses and implemented a query planning mechanism to improve retrieval quality and generate more accurate answers.

<h2 id="day24">Day 24 - 14/05</h2>
Today I continued refactoring the system into a hexagonal architecture integrated with events. I also improved the prompt workflow by automatically identifying patient IDs and names directly through the prompt context, removing the need to manually parse this information in API requests.

<h2 id="day25">Day 25 - 15/05</h2>
I implemented update events for visits, treatments, and diagnostics. Additionally, I reorganized the architecture domains to improve retrieval consistency and maintain proper dependency separation between components. This required refactoring the chunk builders so they correctly adapt to the new domain structure. By the end of the day, the migration to the hexagonal architecture was completed.

---

# Week 6

<h2 id="day26">Day 26 - 18/05</h2>
Today I fixed several smaller bugs and completed the remaining update events before starting the implementation of create events. I also resolved issues affecting the RAG responses, including problems that were causing hallucinations and empty outputs even when the relevant information was already available in the system.

<h2 id="day27">Day 27 - 19/05</h2>
Check and correct the connection with the database through all the app for dependency injection instead of a singleton. I started on implemente the events needed to create all the entities of domain and create the chunks in the vector DB automatically so RAG can use the proper context.

<h2 id="day28">Day 28 - 20/05</h2>
Today I completed the implementation of create events for all the relevant entities in the system. I also conducted thorough testing to ensure that the event-driven architecture is functioning correctly and that all components are properly integrated. Additionally, I started working on improving the documentation to reflect the recent changes in the architecture and workflow.

<h2 id="day29">Day 29 - 21/05</h2>
Today I focused on optimizing the RAG pipeline by implementing more efficient retrieval strategies and improving the scoring mechanism for the cohort-based approach. I also worked on enhancing the documentation to provide clearer explanations of the system architecture and the event-driven workflow, ensuring that it is easier for future developers to understand and maintain the codebase. I also fixed some minor bugs related to the event handling and data synchronization between the main database and the vector database.

<h2 id="day30">Day 30 - 22/05</h2>
Today I introduce the heuristic model to retrieve the risk of theh patient based on the information available in the system. This model uses a set of predefined rules and thresholds to assess the patient's condition and provide a risk score that can be used to prioritize cases and guide clinical decision-making.

---

# Week 7

<h2 id="day31">Day 31 - 25/05</h2>
Today I started working on the interface of the UI, implementing the necessary components to display the RAG responses in a user-friendly manner. And an overall funcionalities that the application could offer, to be able to show it to the customer on Thursday. Additionally, I continued testing the system to identify any remaining issues and ensure that all components are functioning correctly.

<h2 id="day32">Day 32 - 26/05</h2>
I connected properly the UI with the backend API, allowing for real-time interaction and retrieval of RAG responses. I implement websockets to enable dynamic updates to enable the alerts of the risk of the patients displayed in the UI.

<h2 id="day33">Day 33 - 27/05</h2>
I kept connecting the UI with the backend, improving the user experience and ensuring that all functionalities are working as expected. I also prepared a demo to showcase the progress of the project to the customer, highlighting the key features and improvements made during the internship.

<h2 id="day34">Day 34 - 28/05</h2>
We presented the demo to the customer, demonstrating the functionality of the RAG pipeline and the user interface. The feedback received was positive, with some suggestions for further improvements and additional features that could be implemented in the future. I kept on working in a few bugs that were found after the demo and started preparing the final report and presentation for the internship evaluation.

<h2 id="day35">Day 35 - 29/05</h2>
We conducted the last visit with the intership supervisor and we discussed the overall progress of the project and shown the demo. I finish fetching the doctors and the patients with the backend and the frontend so the system is fully functional, without mockup data.

---

# Week 8

<h2 id="day36">Day 36 - 01/06</h2>

<h2 id="day37">Day 37 - 02/06</h2>

<h2 id="day38">Day 38 - 03/06</h2>

<h2 id="day39">Day 39 - 04/06</h2>

<h2 id="day40">Day 40 - 05/06</h2>
