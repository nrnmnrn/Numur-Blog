---
title: "Reflections on My First Year as an AI Engineer: From "Trial by Fire" to a Sustainable Rhythm"
datePublished: Tue Feb 10 2026 02:35:53 GMT+0000 (Coordinated Universal Time)
cuid: cmlfzobq0000002la6n0ib401
slug: reflections-on-my-first-year-as-an-ai-engineer-from-trial-by-fire-to-a-sustainable-rhythm
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/cckf4TsHAuw/upload/6650e3f60ed25f207f497b5d9b2b8c8a.jpeg
tags: spark, career, english, mlops, databricks, ai-engineer, claude-code

---

### **Introduction**

2025 marked my first year in the workforce as a full-time professional.

Though I’ve been in the industry for less than a year, I’ve managed to find a steady rhythm that works for me. I decided to take a moment to look back and organize my thoughts on this journey. Early on, I was caught in a constant loop of "trial and error" and frustration, leaving me with zero mental bandwidth to process what was actually happening. Now that the dust has settled, here’s how it went.

---

### **1\. An Unexpected Start**

Back in university, I specialized in Natural Language Processing (NLP). Naturally, when I saw a game company recruiting for an NLP Engineer, I hit "apply."

Then came the online technical assessment. To my surprise, **the entire test was about Recommendation Systems—not a single question touched on NLP.**

At first, I thought I had simply misread the job description. Since I had also applied for other RecSys roles and had built a few projects in that area, I just buckled down and finished the test.

It wasn’t until the second interview—after re-checking the JD—that I realized the role was officially listed as NLP. During the interview, the hiring manager clarified: they actually needed someone for Recommendation Systems. It turns out there was a clerical error in the job posting. In a strange twist of fate, that mix-up probably filtered out other candidates, and because I happened to have a solid foundation in RecSys, I got the job.

Just like that, I became part of the first wave of AI engineers at a major game company.

---

### **2\. Reality Hits Hard**

The company wanted a RecSys engineer to boost revenue through AI-driven game recommendations. However, since the internal AI team was still in its infancy, I only had one or two colleagues who could offer technical advice.

Over 95% of the project was developed by me alone. Model selection, pipeline design, data cleaning, training, testing, evaluation, and optimizing for speed and memory—it was a one-man show. My collaborators helped me navigate the database schema and explained business requirements, but the technical implementation was entirely on me.

To make things more challenging, the company was just beginning to adopt **Databricks**. No one had prior experience with it. I had to learn how to build MLOps from scratch while simultaneously mastering **Spark** for ETL processes.

In school, I used Pandas for everything. But with millions of users, Pandas would simply crash the memory. Switching to Spark opened up a whole new world of headaches: inexplicably long execution times, "Task not serializable" errors, and the dreaded **OOM (Out of Memory)** errors.

I spent countless nights debugging. My initial strategy was to "Google it" or feed code to Gemini. But it became an endless cycle: fixing one bug only to trigger another, or having Gemini overwrite previous logic. OOM errors were the most soul-crushing because they are notoriously hard to debug. I had to stare at the Spark UI—which is a nightmare for beginners—and guess which part of the logic was causing the bottleneck. One OOM error could easily stall my progress for an entire day.

---

### **3\. A Shift in Strategy**

After numerous late nights, I finally admitted the truth: **This system was currently beyond my capabilities.** I couldn't do this alone without a better approach. I made two key changes:

1. **Finding the Right AI Tools:** Since I wasn't fluent in PySpark syntax, I needed tools that could help translate my logic into correct code efficiently.
    
2. **Systematic Learning:** I stopped "firefighting" and started studying. I bought books on Spark to understand the "why" rather than just looking for quick fixes.
    

The books helped identify common bugs, but since they were often written in Scala while I used PySpark, there was still a gap. However, I finally began to develop a systematic understanding instead of just "spraying and praying."

---

### **4\. Exploring the Tooling Landscape**

I started with **GitHub Copilot**, then tried **Gemini Code Assist**. They were okay for simple tasks, but they struggled with complex, multi-file changes.

Then I tried **Claude Code**, and the experience was night and day.

What impressed me most wasn't just Claude's coding prowess, but its **engineering intuition**. Often, I’d misdiagnose a bug at 'Point A,' but Claude would steer me toward a more pragmatic solution or catch a regression I hadn’t even considered. With the integration of Model Context Protocol (MCP), it felt less like a code completion tool and more like having a senior pair-programmer by my side.

I then discovered Speckit, an open-source tool with tens of thousands of stars on GitHub. Its "Spec-driven development" philosophy was appealing, but after two or three weeks, I found it too rigid.

My conclusion: **As models get smarter, the necessity for over-documentation decreases.** The main pain point of 'Vibe Coding' with earlier tools was the tendency for AI to generate outdated syntax—a challenge that Claude Code, especially when paired with Context7, has largely overcome. Throughout that week, I also explored tools like ContextKit, ClaudeCode Pro, Agent OS, and Plandex, but I ultimately moved past them. With Sonnet 4.5 and Opus 4.5, the error rate has dropped so much that these extra frameworks felt redundant for my current needs.

---

### **5\. Building a Personal Learning System**

Even with powerful tools, I realized a new risk: **If I just blindly accepted what Claude Code suggested, I’d have no idea how my own system worked.** To stay in control, I built a learning system using **Obsidian**. My workflow looks like this:

> **AI Response** → **Daily Learning Log** → **Personal Knowledge Base**

Whenever Claude mentions a technical detail I don’t understand, I ask follow-up questions and document the answers. Obsidian’s "linked notes" feature allows me to turn these scattered insights into a knowledge graph. This helps me find the balance between "being led by the tool" and "truly understanding the tech." I don't need to know every low-level detail, but I must know the trade-offs and risks of the path we're taking.

* *Claude Code x Obsidian: My Second Brain for Engineering*
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1770704111495/6a606835-1d4f-4a97-bc08-bd03149a3d56.jpeg align="center")
    

---

### **6\. My Current Workflow**

Today, my rhythm is much more sustainable:

* **During work:** I develop alongside Claude Code. I use the time saved to dig into the "why" behind its suggestions and log those technical details.
    
* **After work:** I review my logs, write for my blog, or work on side projects and competitions.
    

The biggest shift has been the **sense of control**. I used to be anxious just trying to keep my head above water. Now, I can finish tasks efficiently and reallocate that energy toward long-term value, like optimizing model accuracy or mastering deeper technical nuances.

---

### **7\. The Two Biggest Lessons of the Year**

Looking back, these are the two things that changed everything for me:

#### **1\. Admit what you don’t know**

I used to waste time trying to master every detail of complex systems like Spark. I eventually realized that you can't digest that much information all at once, and if you don't use it, you lose it. Now, I use **Just-In-Time learning**: I build my knowledge base outward from the specific problems I encounter. This makes the information stick because it has context.

#### **2\. Assess your capacity and progress early**

I used to have a "just work harder" mentality. Now, I’ve learned to identify parts of a project that are outside my reach and flag them to the team early. The project impacts more than just me. Communicating early allows the team to adjust together, and it gives me the space to learn properly rather than being pushed by the deadline.

---

### **Closing Thoughts**

This year, I grew from a confused junior into an engineer capable of independently delivering a RecSys project and managing my own workflow.

Beyond the technical skills, the real win was learning **how to learn**, **how to face my own limitations**, and **how to find a balance between work and life.** If you’re currently struggling through your first year, hang in there—it gets better once you find your rhythm.