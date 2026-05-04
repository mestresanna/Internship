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

<h2 id="day17">Day 17 - 05/05</h2>

<h2 id="day18">Day 18 - 06/05</h2>

<h2 id="day19">Day 19 - 07/05</h2>

<h2 id="day20">Day 20 - 08/05</h2>
