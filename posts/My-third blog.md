---
title: From Community Posts to Structured Care Data
date: 2026-04-25
author: Maggie Min
summary: Developing a more structured system to suppoet filtering, maching and reusable care knowledge
tags:
  - StructuredData
  - SystemDesign
  - DatabaseThinking
---
Then, I started thinking more seriously about how the system should actually work. At first, I imagined the platform as a normal online community where users could freely share stories and experiences. However, after thinking more carefully about it, I realised that relying only on free-form posts would create several problems.

If most users only write long discussion posts, other users may struggle to quickly find useful information when using the matching feature. Many important details could become buried under large amounts of text, which would make searching very difficult. Different users may also describe the same issue in completely different ways, which would make filtering and matching less accurate.

Because of this, I started trying to make the platform more structured. Instead of treating every case as one complete post, I decided to separate the information inside each post into different parts. For example, each case would include the pet type, age, temperament, alone time, behaviour issue, routine, and outcome. This structure would not only help users compare cases more easily, but also help the system organise and summarise information more effectively.

This also helped me divide the interface into different entities, such as User, Pet, CareCase, Routine, and Behaviour. I realised that the owner of the same pet may create different posts over time, while the same behaviour issue may also appear across different cases. Another situation is that one post may include multiple behaviour problems at the same time, such as barking, pacing, and scratching at the door. Because of this, the behaviour structure needs to be more flexible so users can filter cases more effectively.

Another important decision was separating the routine structure into its own entity. A routine may include multiple steps, different stages, and different levels of effectiveness. Separating it into its own structure would make the information much clearer and easier to manage.

Because of this, I feel that this kind of structure is very helpful for supporting the platform’s overall functionality. After thinking more carefully about it, I also gained a clearer understanding of the platform’s core features and the different types of content that I could include in the system.
