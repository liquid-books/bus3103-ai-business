---
exports:
  - format: typst
    output: exports/ch01-introduction-to-ai-in-business.pdf
    id: ch01-introduction-to-ai-in-business-pdf
downloads:
  - id: ch01-introduction-to-ai-in-business-pdf
    title: Download Chapter PDF
title: "Chapter 1: Introduction to AI in Business"
subtitle: "Understanding the Foundations of Artificial Intelligence and Its Business Applications"
short_title: "Introduction to AI"
description: |
  An introduction to artificial intelligence for business students, covering AI definitions, categories
  (machine learning, generative AI), business automation, prompt engineering fundamentals, and an
  introduction to privacy and bias considerations.
label: ch01-intro-ai-business
tags:
  - artificial intelligence
  - machine learning
  - generative AI
  - prompt engineering
  - business automation
  - privacy
  - bias
---

# Chapter 1: Introduction to AI in Business

> 📥 [Download this chapter as PDF](./downloads/ch01-introduction-to-ai-in-business.pdf)



:::{figure} ../images/ch01-infographic-ai-business.png
:label: fig-ch01-infographic
:alt: A comprehensive infographic summarizing key concepts in AI for business, including AI categories, machine learning, generative AI, prompt engineering, and ethical considerations
:width: 80%
:align: center

An illustrated overview of the foundational AI concepts covered in this chapter — from defining artificial intelligence to understanding its role in modern business.
:::

:::{epigraph}
"The fear of the LORD is the beginning of wisdom, and knowledge of the Holy One is understanding."

-- Proverbs 9:10 (NIV)
:::

Artificial intelligence is no longer a futuristic concept confined to science fiction novels and research laboratories. It is here — embedded in the tools we use daily, transforming the industries we work in, and reshaping the very nature of business itself. From the algorithms that recommend products on Amazon to the chatbots that handle customer service inquiries, AI has become an invisible but powerful force in the modern economy.

For students preparing to enter the business world, understanding AI is not optional — it is essential. But understanding AI as a business professional is fundamentally different from understanding it as a computer scientist. You do not need to write neural network code from scratch. What you need is the ability to recognize where AI creates value, evaluate AI-powered tools critically, communicate effectively with technical teams, and make ethical decisions about how AI is deployed in your organization.

This chapter lays the foundation for your journey into AI for business. We will define artificial intelligence and its major categories, explore how businesses are already using AI to automate processes and gain competitive advantages, introduce the art and science of prompt engineering, and begin an important conversation about privacy and bias — two issues that every business leader must understand in the age of AI.

As students at Palm Beach Atlantic University, you bring a unique perspective to this conversation. Your education is grounded in Christian values — values that emphasize truth, stewardship, human dignity, and ethical responsibility. These values are not obstacles to innovation; they are exactly what the world of AI needs. As we explore these powerful technologies together, we will continually ask: How do we use these tools in ways that honor God, serve others, and promote human flourishing?

## What Is Artificial Intelligence?

### Defining AI: More Than Just "Smart Machines"

:::{prf:definition} Artificial Intelligence
:label: def-ai

Artificial intelligence (AI) refers to the development of computer systems that can perform tasks typically requiring human intelligence. These tasks include learning from data, recognizing patterns, making decisions, understanding natural language, perceiving visual information, and generating creative content.
:::

The term "artificial intelligence" was coined in 1956 by John McCarthy at the Dartmouth Conference, a landmark workshop that brought together researchers who believed that "every aspect of learning or any other feature of intelligence can in principle be so precisely described that a machine can be made to simulate it." Nearly seven decades later, that vision has been realized in ways McCarthy could scarcely have imagined.

But defining AI precisely is more challenging than it appears. The field encompasses a vast range of technologies, from simple rule-based systems that follow pre-programmed instructions to sophisticated deep learning models that can generate human-like text, create photorealistic images, and even write computer code. To make sense of this landscape, we need to understand several key distinctions.

:::{figure} ../images/ch01-ai-categories-hierarchy.png
:label: fig-ch01-ai-categories
:alt: Hierarchical diagram showing AI categories from Artificial Intelligence to Machine Learning to Deep Learning to Generative AI, with Narrow AI, General AI, and Superintelligence spectrum
:width: 80%
:align: center

The hierarchy of AI categories — from the broadest concept of Artificial Intelligence down to specific subfields like Machine Learning, Deep Learning, and Generative AI. Understanding this hierarchy is essential for evaluating AI tools and solutions.
:::

### Narrow AI vs. General AI

::::{tab-set}
:::{tab-item} Narrow AI (ANI)
**Narrow AI** (also called Artificial Narrow Intelligence or "weak AI") refers to AI systems designed to perform a specific task or a narrow set of related tasks. Every AI system in commercial use today is narrow AI.

**Examples:**
- Siri and Alexa (voice assistants)
- Netflix recommendation algorithms
- Spam email filters
- Self-driving car navigation systems
- ChatGPT (language generation)
- Medical imaging diagnostic tools

Narrow AI can be extraordinarily powerful within its domain — a chess AI can defeat any human grandmaster — but it cannot transfer that expertise to an unrelated task like writing poetry or diagnosing diseases.
:::

:::{tab-item} General AI (AGI)
**Artificial General Intelligence** (AGI), sometimes called "strong AI," refers to a hypothetical AI system that possesses the full range of human cognitive abilities. An AGI could learn any intellectual task that a human can, transfer knowledge between domains, reason abstractly, and adapt to entirely new situations without specific training.

AGI does not yet exist. Despite dramatic advances in AI capabilities, no system today demonstrates true general intelligence. Estimates for when AGI might be achieved vary wildly — from a few years to several decades to "possibly never."

The pursuit of AGI raises profound philosophical and theological questions about the nature of intelligence, consciousness, and what it means to be human — questions we will return to throughout this course.
:::

:::{tab-item} Superintelligence (ASI)
**Artificial Superintelligence** (ASI) is a theoretical concept referring to AI that surpasses human intelligence in virtually every domain — scientific creativity, social skills, general wisdom, and more.

ASI remains firmly in the realm of speculation, but it has been the subject of serious discussion among AI researchers, philosophers, and ethicists. Thinkers like Nick Bostrom (author of *Superintelligence*) have argued that the development of ASI could pose existential risks to humanity if not carefully managed.

For our purposes in this course, we will focus on narrow AI — the technology that is transforming business today — while keeping an eye on the trajectory toward more capable systems.
:::
::::

### The AI Spectrum: From Rules to Learning

Not all AI works the same way. It is helpful to think of AI technologies as existing on a spectrum, from simple rule-based systems to sophisticated learning algorithms.

:::{mermaid}
:label: fig-ch01-ai-spectrum

graph LR
    A["Rule-Based Systems<br/>(If-Then Logic)"] --> B["Expert Systems<br/>(Knowledge Bases)"]
    B --> C["Machine Learning<br/>(Pattern Recognition)"]
    C --> D["Deep Learning<br/>(Neural Networks)"]
    D --> E["Generative AI<br/>(Content Creation)"]

    style A fill:#e8f4fd,stroke:#1976d2
    style B fill:#e3f2fd,stroke:#1976d2
    style C fill:#bbdefb,stroke:#1976d2
    style D fill:#90caf9,stroke:#1565c0
    style E fill:#64b5f6,stroke:#0d47a1
:::

:::{list-table} The AI Technology Spectrum
:label: tbl-ch01-ai-spectrum
:header-rows: 1

* - Technology
  - How It Works
  - Business Example
  - Era
* - Rule-Based Systems
  - Follows pre-programmed if-then rules
  - Tax preparation software
  - 1960s–present
* - Expert Systems
  - Encodes domain expert knowledge into decision rules
  - Medical diagnosis assistants
  - 1970s–1990s
* - Machine Learning
  - Learns patterns from data without explicit programming
  - Fraud detection, product recommendations
  - 2000s–present
* - Deep Learning
  - Uses multi-layered neural networks for complex pattern recognition
  - Voice recognition, image classification
  - 2010s–present
* - Generative AI
  - Creates new content (text, images, code, audio) based on training data
  - ChatGPT, DALL-E, Midjourney
  - 2020s–present
:::

## Categories of AI: Machine Learning and Generative AI

### Machine Learning: Learning from Data

:::{prf:definition} Machine Learning
:label: def-ml

Machine learning (ML) is a subset of artificial intelligence in which computer systems learn to perform tasks by identifying patterns in data, rather than being explicitly programmed with rules. The system improves its performance as it is exposed to more data over time.
:::

Machine learning is the engine that powers most modern AI applications. Rather than telling a computer exactly what to do in every situation, ML allows the computer to learn from examples. Feed it thousands of emails labeled "spam" or "not spam," and it learns to identify spam on its own. Show it millions of product purchases and customer profiles, and it learns to recommend products that customers are likely to buy.

#### The Three Types of Machine Learning

::::{grid} 1 1 3 3
:::{card} Supervised Learning
:class-header: bg-primary text-white

**Learning from labeled examples**
^^^
The algorithm is trained on a dataset where the correct answer is provided for each example. It learns to map inputs to outputs.

**Business applications:**
- Email spam classification
- Credit scoring and loan approvals
- Sales forecasting
- Customer churn prediction
- Medical diagnosis from imaging

**Analogy:** Like a student learning from a textbook with an answer key — they study the questions and correct answers, then apply what they learned to new questions.
:::

:::{card} Unsupervised Learning
:class-header: bg-success text-white

**Discovering hidden patterns**
^^^
The algorithm explores data without labeled answers, seeking to find natural groupings, patterns, or structures.

**Business applications:**
- Customer segmentation
- Market basket analysis
- Anomaly detection (fraud)
- Topic modeling for documents
- Social network analysis

**Analogy:** Like sorting a pile of photographs into groups without being told what the categories should be — you naturally group by subject, color, or location.
:::

:::{card} Reinforcement Learning
:class-header: bg-warning text-dark

**Learning through trial and error**
^^^
The algorithm learns by interacting with an environment, receiving rewards for good actions and penalties for bad ones.

**Business applications:**
- Dynamic pricing optimization
- Inventory management
- Robotic warehouse automation
- Ad placement optimization
- Game-playing AI (AlphaGo)

**Analogy:** Like training a dog — you reward desired behaviors and correct undesired ones, and the dog gradually learns what to do.
:::
::::

:::{figure} ../images/ch01-ml-types-comparison.png
:label: fig-ch01-ml-types
:alt: A comparison diagram showing the three types of machine learning - supervised, unsupervised, and reinforcement learning - with business examples for each
:width: 80%
:align: center

The three major categories of machine learning, each suited to different business problems. Understanding which type to apply is a key competency for business leaders working with AI.
:::

#### How Machine Learning Works: A Business Perspective

You do not need to understand the mathematics behind gradient descent or backpropagation to be an effective business leader in the AI era. What you do need to understand is the general process by which ML systems are developed and deployed:

:::{mermaid}
:label: fig-ch01-ml-pipeline

graph TD
    A["1. Define the Business Problem"] --> B["2. Collect & Prepare Data"]
    B --> C["3. Choose & Train Model"]
    C --> D["4. Evaluate Performance"]
    D --> E{"Acceptable?"}
    E -->|No| C
    E -->|Yes| F["5. Deploy to Production"]
    F --> G["6. Monitor & Maintain"]
    G --> B

    style A fill:#e8f4fd,stroke:#1976d2
    style F fill:#c8e6c9,stroke:#388e3c
:::

1. **Define the Business Problem.** What decision are you trying to improve? What outcome do you want to predict? The most common reason ML projects fail is not technical — it is a poorly defined business problem.

2. **Collect and Prepare Data.** ML systems learn from data, and the quality of that data determines the quality of the results. This step typically consumes 60-80% of the total project effort. Data must be collected, cleaned, labeled (for supervised learning), and formatted.

3. **Choose and Train the Model.** Data scientists select an appropriate algorithm and train it on the prepared data. Training involves feeding the data through the model and adjusting its parameters to minimize errors.

4. **Evaluate Performance.** The model is tested on data it has never seen before to assess how well it generalizes. Key metrics include accuracy, precision, recall, and F1 score.

5. **Deploy to Production.** The trained model is integrated into business systems where it can make predictions on new data in real time.

6. **Monitor and Maintain.** ML models can degrade over time as the data they encounter changes (a phenomenon called "model drift"). Ongoing monitoring and periodic retraining are essential.

:::{important}
**The Data Quality Principle:** An AI system is only as good as the data it learns from. The business phrase "garbage in, garbage out" has never been more relevant than in the age of machine learning. As business leaders, ensuring data quality, representativeness, and ethical sourcing is one of your most important responsibilities.
:::

### Generative AI: Creating New Content

:::{prf:definition} Generative AI
:label: def-genai

Generative AI refers to artificial intelligence systems that can create new content — including text, images, audio, video, and code — based on patterns learned from training data. Unlike traditional AI systems that classify or predict, generative AI produces original outputs that did not previously exist.
:::

Generative AI has captured the world's attention since the release of ChatGPT in November 2022. In just two months, ChatGPT reached 100 million users — the fastest-growing consumer application in history. But ChatGPT is just one manifestation of a broader technological revolution.

#### The Generative AI Landscape

:::{list-table} Major Generative AI Categories and Tools
:label: tbl-ch01-genai-landscape
:header-rows: 1

* - Category
  - What It Generates
  - Key Tools
  - Business Applications
* - Text Generation
  - Written content, code, analysis
  - ChatGPT, Claude, Gemini, Perplexity
  - Content marketing, customer service, coding assistance, research
* - Image Generation
  - Photorealistic images, illustrations, designs
  - DALL-E, Midjourney, Adobe Firefly, Stable Diffusion
  - Marketing materials, product mockups, advertising creative
* - Audio Generation
  - Speech, music, sound effects
  - ElevenLabs, Suno, Udio
  - Voiceovers, podcasts, accessibility, customer service
* - Video Generation
  - Video clips, animations
  - Sora (OpenAI), Runway, Synthesia
  - Marketing videos, training content, product demos
* - Code Generation
  - Software code, applications
  - GitHub Copilot, Cursor, Replit AI
  - Software development, automation, rapid prototyping
:::

#### How Generative AI Works: The Transformer Architecture

The breakthrough behind modern generative AI is the **transformer architecture**, introduced in the landmark 2017 paper "Attention Is All You Need" by researchers at Google. Transformers process text (or other data) by paying "attention" to the relationships between all parts of the input simultaneously, rather than processing it sequentially.

:::{figure} ../images/ch01-transformer-simplified.png
:label: fig-ch01-transformer
:alt: A simplified diagram showing how the transformer architecture processes input text through attention mechanisms to generate output text
:width: 80%
:align: center

A simplified view of the transformer architecture that powers large language models. The "attention mechanism" allows the model to consider the relationships between all words in a sentence simultaneously.
:::

Large language models (LLMs) like ChatGPT are built on the transformer architecture and trained on vast corpora of text data. During training, the model learns statistical patterns about how words, sentences, and ideas relate to each other. When you provide a prompt, the model generates a response by predicting the most likely sequence of words based on those learned patterns.

:::{warning}
**LLMs Do Not "Understand" in the Human Sense.** Large language models are remarkably capable at producing coherent, contextually appropriate text. But they operate through pattern matching and statistical prediction — they do not truly comprehend meaning, possess beliefs, or have experiences. This distinction matters for business applications: LLMs can generate impressively fluent text that is factually incorrect (a phenomenon called "hallucination"). Always verify AI-generated content before using it in business decisions.
:::

## AI in Business: Automation and Transformation

### The Business Case for AI

:::{figure} ../images/ch01-business-automation-spectrum.png
:label: fig-ch01-automation-spectrum
:alt: Business automation spectrum showing progression from manual processes through rule-based automation, ML-assisted, AI-augmented decision making, to autonomous AI systems
:width: 80%
:align: center

The business automation spectrum — from fully manual processes to autonomous AI systems. Most organizations today are somewhere in the middle, using AI to augment rather than replace human decision-making.
:::

Why are businesses investing billions of dollars in AI? The answer lies in AI's ability to enhance efficiency, improve decision-making, personalize customer experiences, and create entirely new products and services.

:::{list-table} AI Business Impact by Function
:label: tbl-ch01-ai-business-impact
:header-rows: 1

* - Business Function
  - AI Application
  - Impact
  - Example Company
* - Marketing
  - Personalized content, customer segmentation, predictive analytics
  - 20-30% increase in campaign effectiveness
  - Netflix, Spotify
* - Sales
  - Lead scoring, demand forecasting, conversational AI
  - 50% increase in qualified leads
  - Salesforce Einstein
* - Operations
  - Supply chain optimization, predictive maintenance, quality control
  - 15-25% reduction in operational costs
  - Amazon, Siemens
* - Finance
  - Fraud detection, algorithmic trading, risk assessment
  - 60-70% reduction in fraud losses
  - JPMorgan Chase, PayPal
* - Human Resources
  - Resume screening, employee engagement analysis, skills assessment
  - 75% reduction in time-to-hire
  - LinkedIn, HireVue
* - Customer Service
  - Chatbots, sentiment analysis, automated ticket routing
  - 40% reduction in support costs
  - Zendesk, Intercom
:::

### Case Study: How Starbucks Uses AI

Starbucks provides an excellent example of how a large company integrates AI across its operations. Their AI platform, "Deep Brew," powers multiple aspects of the business:

:::{dropdown} Deep Brew in Action
:open: true

**Personalized Recommendations.** The Starbucks mobile app uses machine learning to analyze each customer's purchase history, time of day, weather conditions, and local store inventory to make personalized drink recommendations. This personalization engine drives a significant portion of mobile orders.

**Predictive Inventory Management.** AI models predict demand for each product at each store, accounting for variables like weather, local events, day of the week, and seasonal trends. This reduces waste and ensures popular items are always in stock.

**Labor Optimization.** Deep Brew helps managers schedule staff by predicting busy periods based on historical data and external factors. This ensures adequate coverage during peak times while controlling labor costs.

**Equipment Maintenance.** IoT sensors on espresso machines and other equipment feed data to AI systems that predict when maintenance is needed before a breakdown occurs, reducing downtime and repair costs.

The result? Starbucks has reported that AI-driven personalization has increased customer spending by 3x in some channels and reduced waste by over 30% in pilot stores.
:::

### Case Study: AI at JPMorgan Chase — COiN

JPMorgan Chase's Contract Intelligence (COiN) platform demonstrates AI's transformative potential in finance. The system uses natural language processing and machine learning to review commercial loan agreements — a task that previously required approximately 360,000 hours of lawyer time annually.

COiN can review documents in seconds, extracting key data points with greater accuracy than human reviewers. The system processes 12,000 annual commercial credit agreements, identifying over 150 relevant attributes per document. What once took lawyers months of tedious work is now accomplished in hours, freeing legal professionals to focus on higher-value advisory work.

:::{tip}
**AI Replaces Tasks, Not Jobs (Usually).** Notice that COiN did not eliminate JPMorgan's legal department. It automated the most tedious, repetitive aspects of legal work, allowing lawyers to focus on tasks that require human judgment, creativity, and relationship skills. This "task displacement rather than job displacement" pattern is typical of how AI affects the workplace.
:::

### Case Study: Zara's AI-Powered Fast Fashion

Zara, the Spanish fashion retailer, uses AI throughout its supply chain to maintain its competitive advantage of bringing new designs from concept to store shelf in just two weeks — compared to six months for traditional retailers.

**Trend Prediction.** Zara's AI systems analyze social media posts, fashion blogs, runway shows, and sales data to identify emerging trends before they go mainstream. Natural language processing parses millions of social media conversations to detect rising interest in specific styles, colors, or materials.

**Design Assistance.** AI tools help designers create new garments by suggesting fabric combinations, color palettes, and style elements based on trend analysis. Human designers retain creative control, but AI dramatically accelerates the ideation process.

**Demand Forecasting.** Machine learning models predict demand for each SKU at each store location, enabling Zara to produce smaller initial batches and restock quickly based on actual sales data, rather than overproducing based on forecasts.

**Dynamic Pricing.** AI algorithms optimize markdown timing and pricing to maximize revenue while clearing inventory efficiently.

:::{figure} ../images/ch01-industry-ai-applications.png
:label: fig-ch01-industry-applications
:alt: Grid showing AI applications across six industry sectors — healthcare, finance, retail, manufacturing, marketing, and HR — with specific use cases for each
:width: 80%
:align: center

AI applications across major industry sectors. Every business function is being transformed by AI, creating opportunities for competitive advantage and operational efficiency.
:::

### Small Business AI Applications

AI is not exclusively for large corporations. Small and medium-sized businesses are increasingly adopting AI tools that were once available only to enterprises with massive technology budgets:

::::{grid} 1 1 2 2
:::{card} Marketing & Content
- **Jasper AI / Copy.ai:** Generate marketing copy, social media posts, email campaigns
- **Canva AI:** Design marketing materials with AI-assisted tools
- **HubSpot AI:** Automated email marketing and lead nurturing
- **Buffer AI Assistant:** Social media content scheduling and optimization
:::

:::{card} Operations & Productivity
- **QuickBooks AI:** Automated bookkeeping and financial forecasting
- **Grammarly Business:** AI-powered writing assistance for teams
- **Notion AI:** Automated note-taking, summarization, project management
- **Zapier AI:** Automated workflow connections between apps
:::

:::{card} Customer Service
- **Tidio / Intercom:** AI chatbots for customer support
- **Freshdesk AI:** Automated ticket routing and response suggestions
- **CallRail:** AI-powered call tracking and conversation analysis
- **Gorgias:** E-commerce customer support automation
:::

:::{card} Sales & Analytics
- **Crystal Knows:** AI-powered personality insights for sales
- **Gong.io:** AI analysis of sales calls for coaching
- **Google Analytics 4:** AI-powered website analytics and predictions
- **Tableau AI:** Automated data visualization and insights
:::
::::

## Prompt Engineering: The New Business Literacy

### What Is Prompt Engineering?

:::{prf:definition} Prompt Engineering
:label: def-prompt-engineering

Prompt engineering is the practice of designing and refining text inputs (prompts) given to AI systems — particularly large language models — to elicit desired outputs. Effective prompt engineering involves understanding how AI models interpret instructions and structuring prompts to maximize the quality, relevance, and accuracy of responses.
:::

In the age of generative AI, prompt engineering has emerged as a critical skill for business professionals. The quality of output you get from an AI system depends enormously on the quality of the instructions you provide. A vague, poorly structured prompt will produce vague, poorly structured results. A clear, detailed, well-structured prompt will produce clear, detailed, useful results.

Think of prompt engineering as the new "search literacy." Just as the rise of Google required people to develop skills in formulating effective search queries, the rise of generative AI requires people to develop skills in formulating effective prompts.

### The Anatomy of an Effective Prompt

Effective prompts typically include several key components:

:::{figure} ../images/ch01-prompt-anatomy.png
:label: fig-ch01-prompt-anatomy
:alt: A diagram showing the key components of an effective AI prompt, including role, context, task, format, constraints, and examples
:width: 80%
:align: center

The anatomy of an effective AI prompt. Each component contributes to generating a more accurate and useful response.
:::

:::{list-table} Components of an Effective Prompt
:label: tbl-ch01-prompt-components
:header-rows: 1

* - Component
  - Purpose
  - Example
* - **Role**
  - Establish the AI's persona and expertise level
  - "You are a senior financial analyst specializing in retail industry trends."
* - **Context**
  - Provide background information the AI needs
  - "Our company is a mid-size retailer with $50M annual revenue considering expanding into e-commerce."
* - **Task**
  - Clearly state what you want the AI to produce
  - "Create a competitive analysis comparing our top three e-commerce platform options."
* - **Format**
  - Specify the desired output structure
  - "Present as a comparison table with rows for each platform and columns for cost, features, scalability, and ease of integration."
* - **Constraints**
  - Set boundaries and requirements
  - "Keep the analysis focused on platforms supporting fewer than 10,000 SKUs. Budget limit: $500/month."
* - **Examples**
  - Show the AI what good output looks like
  - "Here is an example of the format I want: [example]"
:::

### Prompting Techniques for Business

#### Zero-Shot Prompting
The simplest approach — provide a task with no examples.

```text
Summarize the key risks of implementing an AI chatbot for customer 
service in a healthcare organization. Focus on regulatory compliance, 
patient privacy, and liability concerns.
```

#### Few-Shot Prompting
Provide examples of desired input-output pairs before your actual task.

```text
Classify the following customer reviews as Positive, Negative, or Neutral:

Review: "The product exceeded my expectations! Fast shipping too."
Classification: Positive

Review: "It works, but nothing special for the price."
Classification: Neutral

Review: "Terrible quality. Broke after one week. Want a refund."
Classification: Negative

Review: "I've been using this software for three months and it has 
completely transformed our inventory management process."
Classification:
```

#### Chain-of-Thought Prompting
Ask the AI to reason step by step before providing a final answer.

```text
A small retail business has monthly revenue of $120,000 and is 
considering implementing an AI-powered inventory management system 
that costs $2,000/month. Historical data shows similar businesses 
have reduced inventory costs by 15-20% with such systems. Their 
current monthly inventory cost is $40,000. 

Think through this step by step:
1. Calculate the potential savings range
2. Determine the net benefit after the system cost
3. Calculate the ROI
4. Recommend whether to proceed and explain your reasoning
```

#### Role-Based Prompting
Assign the AI a specific professional role to shape its perspective and language.

```text
You are a Christian business ethics professor at a university. A 
student asks you: "Is it ethical for a company to use AI to make 
hiring decisions without telling candidates?" 

Provide a thoughtful response that considers:
- Biblical principles of honesty and transparency
- Legal requirements (EEOC guidelines)
- Practical business considerations
- The dignity of job applicants as people made in God's image
```

### Common Prompting Mistakes

:::{warning}
**Avoid These Common Mistakes:**

1. **Being too vague.** "Tell me about AI in business" → Too broad. Specify what aspect, what industry, what depth.
2. **Overloading the prompt.** Asking for too many things in one prompt leads to shallow responses. Break complex tasks into steps.
3. **Not specifying format.** If you want a table, ask for a table. If you want bullet points, say so. AI will default to prose paragraphs otherwise.
4. **Ignoring the audience.** "Explain machine learning" could produce a PhD-level explanation or a kindergarten-level one. Specify who the explanation is for.
5. **Treating AI output as final.** AI-generated content is a first draft. Always review, verify facts, and edit for your specific context.
6. **Not iterating.** If the first response isn't right, refine your prompt rather than starting over. AI conversations are iterative.
:::

### Practical Exercise: Prompt Comparison

Consider these two prompts asking for the same information:

::::{tab-set}
:::{tab-item} Weak Prompt
```text
Write something about using AI in marketing.
```

**Problems:**
- No role assignment
- No specific focus
- No format specification
- No audience definition
- No length guidance
- No constraints
:::

:::{tab-item} Strong Prompt
```text
You are a digital marketing strategist with 10 years of experience 
in retail. Create a concise action plan (500-700 words) for a small 
clothing boutique owner who wants to start using AI tools in their 
marketing. The owner has no technical background and a monthly 
marketing budget of $500.

Include:
1. Three specific AI tools they should try first (with pricing)
2. A realistic 30-day implementation timeline
3. Expected results they can measure
4. One potential risk to watch for

Write in a practical, jargon-free style. Use bullet points for 
the action items.
```

**Why this works:**
- Clear role and expertise level
- Specific audience with constraints
- Defined format and length
- Actionable deliverables
- Measurable outcomes requested
:::
::::

## Privacy and Bias: An Introduction

### Why Privacy Matters in the AI Era

:::{epigraph}
"The prudent see danger and take refuge, but the simple keep going and pay the penalty."

-- Proverbs 27:12 (NIV)
:::

AI systems are fundamentally data-driven. They learn from data, they process data, and they make decisions based on data. This creates inherent privacy concerns that every business professional must understand.

:::{figure} ../images/ch01-privacy-data-lifecycle.png
:label: fig-ch01-privacy-lifecycle
:alt: Circular data privacy lifecycle diagram showing stages from data collection through storage, AI processing, analysis, sharing, and deletion with regulatory checkpoints
:width: 80%
:align: center

The data privacy lifecycle in AI-driven organizations. Each stage presents unique privacy considerations and regulatory requirements that business leaders must understand and manage.
:::

#### Data Collection and Consent

Modern AI systems often require vast amounts of data to function effectively. This data frequently includes personal information — customer purchase histories, browsing behavior, demographic information, health records, financial data, and more. The ethical and legal questions surrounding this data are profound:

- **Informed consent.** Do customers understand what data is being collected and how AI systems will use it?
- **Purpose limitation.** Is data collected for one purpose being used for another without consent?
- **Data minimization.** Is the organization collecting only the data it truly needs, or is it hoarding data "just in case"?
- **Right to be forgotten.** Can individuals request deletion of their data from AI training sets?

#### Key Privacy Regulations

:::{list-table} Major Data Privacy Regulations
:label: tbl-ch01-privacy-regulations
:header-rows: 1

* - Regulation
  - Jurisdiction
  - Key Provisions
  - AI Relevance
* - GDPR
  - European Union
  - Right to access, deletion, portability; consent requirements; data breach notification
  - Right to explanation of automated decisions; restrictions on AI profiling
* - CCPA/CPRA
  - California, USA
  - Right to know what data is collected; right to opt-out of data sales; right to deletion
  - Applies to AI-driven personalization and profiling
* - HIPAA
  - USA (Healthcare)
  - Protection of health information; security requirements; breach notification
  - Strict limits on using health data for AI training
* - FERPA
  - USA (Education)
  - Student record privacy; parental consent requirements
  - Limits use of student data in educational AI tools
* - EU AI Act
  - European Union
  - Risk-based classification of AI systems; transparency requirements; prohibited practices
  - First comprehensive AI-specific regulation globally
:::

:::{important}
**The EU AI Act (2024)** is the world's first comprehensive AI regulation. It classifies AI systems by risk level (unacceptable, high, limited, minimal) and imposes corresponding requirements. Business students should understand this framework, as it is likely to influence AI regulation worldwide — much as GDPR influenced global privacy law.
:::

#### Case Study: Cambridge Analytica

The Cambridge Analytica scandal (2018) remains one of the most important cautionary tales about AI and privacy. The political consulting firm harvested personal data from approximately 87 million Facebook users through a personality quiz app. The data — collected without users' meaningful consent — was used to build AI-driven psychographic profiles for targeted political advertising during the 2016 U.S. presidential election and the Brexit referendum.

The fallout was severe: Facebook (now Meta) paid a $5 billion FTC fine — the largest privacy penalty in U.S. history. Cambridge Analytica went bankrupt. Public trust in social media data practices plummeted. And the scandal accelerated the passage of privacy legislation worldwide.

:::{note}
**Lesson for Business Leaders:** The short-term competitive advantages of aggressive data collection practices can be utterly dwarfed by the legal, financial, and reputational consequences of privacy violations. Building a culture of ethical data stewardship is not just the right thing to do — it is sound business strategy.
:::

### Understanding AI Bias

:::{prf:definition} AI Bias
:label: def-ai-bias

AI bias refers to systematic errors in AI system outputs that result in unfair outcomes for certain groups of people. Bias can originate from biased training data, flawed algorithm design, biased human decisions during development, or the broader social and historical context in which the system operates.
:::

AI bias is one of the most critical challenges facing businesses deploying AI systems. Because AI learns from historical data — and historical data reflects historical inequities — AI systems can perpetuate, amplify, and even automate discrimination.

:::{figure} ../images/ch01-ai-bias-sources.png
:label: fig-ch01-bias-sources
:alt: Diagram showing four sources of AI bias — data bias, algorithmic bias, human bias, and societal bias — flowing into an AI system and producing biased outputs
:width: 80%
:align: center

The four primary sources of AI bias and how they propagate through the AI pipeline. Understanding these sources is the first step toward building fairer AI systems.
:::

#### Sources of AI Bias

:::{mermaid}
:label: fig-ch01-bias-sources

graph TD
    A["AI Bias"] --> B["Data Bias"]
    A --> C["Algorithmic Bias"]
    A --> D["Human Bias"]
    A --> E["Societal Bias"]

    B --> B1["Unrepresentative samples"]
    B --> B2["Historical discrimination in data"]
    B --> B3["Missing data for minority groups"]

    C --> C1["Optimization for wrong metrics"]
    C --> C2["Feature selection biases"]

    D --> D1["Developer assumptions"]
    D --> D2["Labeling biases"]

    E --> E1["Structural inequities"]
    E --> E2["Cultural biases encoded in language"]

    style A fill:#ff9800,stroke:#e65100
    style B fill:#fff3e0,stroke:#ff9800
    style C fill:#fff3e0,stroke:#ff9800
    style D fill:#fff3e0,stroke:#ff9800
    style E fill:#fff3e0,stroke:#ff9800
:::

#### Case Study: Amazon's AI Recruiting Tool

In 2018, Reuters reported that Amazon had scrapped an AI recruiting tool that showed significant bias against women. The system was trained on resumes submitted to the company over a ten-year period — a period during which the technology industry was overwhelmingly male. The AI learned to associate "male" characteristics with success:

- It penalized resumes that included the word "women's" (as in "women's chess club captain")
- It downgraded graduates of all-women's colleges
- It favored language patterns more common in male-written resumes

Amazon's engineers attempted to correct the bias, but ultimately concluded that they could not guarantee the system would not find other ways to discriminate. The project was abandoned.

:::{tip}
**The Lesson:** AI systems do not have a moral compass. They optimize for whatever patterns exist in the training data. If the data reflects historical discrimination, the AI will learn to discriminate. This is why diverse development teams, careful data curation, and ongoing bias auditing are essential.
:::

#### Case Study: Healthcare Algorithm Bias

A 2019 study published in *Science* revealed that a widely used healthcare algorithm — used by hospitals across the United States to predict which patients need extra medical care — exhibited significant racial bias. The algorithm used healthcare spending as a proxy for healthcare needs. But because Black patients in America historically have had less access to healthcare (and therefore lower healthcare spending), the algorithm systematically underestimated the healthcare needs of Black patients.

The result: Black patients who were equally as sick as white patients were assigned lower risk scores and received less additional care. The study estimated that eliminating this bias would increase the percentage of Black patients receiving extra care from 17.7% to 46.5%.

### A Christian Perspective on Privacy and Bias

As Christians entering the business world, we have a unique and important perspective on these issues:

:::{note}
**Imago Dei and Human Dignity.** Scripture teaches that every human being is created in the image of God (Genesis 1:27). This fundamental truth demands that we design and deploy AI systems that respect the inherent dignity of every person — regardless of race, gender, socioeconomic status, or any other characteristic. AI systems that systematically disadvantage certain groups are not merely bad technology — they are affronts to human dignity.

**Truth and Transparency.** "The LORD detests lying lips, but he delights in people who are trustworthy" (Proverbs 12:22). Businesses have an obligation to be transparent about how they use AI and personal data. Hiding AI-driven decision-making behind a veil of "proprietary algorithms" fails the test of truthfulness.

**Stewardship.** We are called to be faithful stewards of the resources and influence entrusted to us (Matthew 25:14-30). This includes the data entrusted to us by customers and the powerful technologies at our disposal. Stewardship demands that we use these resources responsibly and for the benefit of others, not merely for profit maximization.

**Justice.** "He has shown you, O mortal, what is good. And what does the LORD require of you? To act justly and to love mercy and to walk humbly with your God" (Micah 6:8). When AI systems produce unjust outcomes — whether through biased hiring, discriminatory lending, or unequal healthcare — we have a responsibility to identify, correct, and prevent these harms.
:::

## The AI-Ready Business Professional

### Skills for the AI Era

What does it mean to be "AI-ready" as a business professional? It does not mean becoming a data scientist or software engineer. It means developing a specific set of competencies that enable you to work effectively alongside AI:

::::{grid} 1 1 2 2
:::{card} Technical Literacy
- Understand AI categories and capabilities
- Evaluate AI tools for specific business needs
- Write effective prompts for generative AI
- Interpret AI-generated insights and recommendations
- Recognize limitations and failure modes
:::

:::{card} Strategic Thinking
- Identify business problems that AI can solve
- Assess build-vs-buy-vs-partner decisions
- Calculate ROI for AI investments
- Understand competitive implications of AI adoption
- Plan AI implementation roadmaps
:::

:::{card} Ethical Leadership
- Evaluate AI systems for bias and fairness
- Ensure compliance with privacy regulations
- Advocate for transparent AI practices
- Balance innovation with responsibility
- Apply Christian values to technology decisions
:::

:::{card} Communication
- Explain AI capabilities to non-technical stakeholders
- Collaborate effectively with data science teams
- Present AI-driven insights to decision-makers
- Manage change when AI transforms workflows
- Build trust in AI-augmented processes
:::
::::

### The Human-AI Collaboration Framework

The most successful organizations don't replace humans with AI — they design workflows that leverage the unique strengths of both:

:::{list-table} Human vs. AI Strengths
:label: tbl-ch01-human-ai
:header-rows: 1

* - Capability
  - Human Advantage
  - AI Advantage
* - Pattern Recognition
  - Recognizes novel, unprecedented patterns
  - Finds patterns in massive datasets at scale
* - Creativity
  - Generates truly novel ideas, empathy-driven design
  - Generates variations and combinations rapidly
* - Decision Making
  - Considers ethics, context, relationships
  - Processes data objectively, consistently
* - Communication
  - Understands nuance, emotion, culture
  - Processes language at massive scale, 24/7
* - Learning
  - Transfers knowledge across wildly different domains
  - Learns from millions of examples rapidly
* - Judgment
  - Moral reasoning, wisdom, accountability
  - Optimizes for defined objectives consistently
:::

:::{important}
**The Complementarity Principle:** The most powerful applications of AI in business are not those that replace human workers entirely, but those that combine AI's speed, scale, and consistency with human creativity, judgment, and ethical reasoning. Your goal is not to compete with AI — it is to become exceptional at the things AI cannot do.
:::

## Chapter Summary

This chapter has introduced the foundational concepts you need to begin your journey into AI for business:

1. **Artificial intelligence** encompasses a range of technologies, from simple rule-based systems to sophisticated generative AI, all designed to perform tasks typically requiring human intelligence.
2. **Machine learning** — the engine behind most modern AI — enables systems to learn from data rather than being explicitly programmed, with supervised, unsupervised, and reinforcement learning as the three major categories.
3. **Generative AI** represents the latest frontier, with systems like ChatGPT, DALL-E, and Gemini capable of creating new text, images, audio, and code.
4. **AI is transforming every business function** — from marketing and sales to operations and finance — creating both opportunities and challenges.
5. **Prompt engineering** is emerging as a critical business literacy skill, enabling professionals to interact effectively with AI systems.
6. **Privacy and bias** are fundamental challenges that demand attention from every business leader deploying AI systems.
7. **As Christians**, we bring essential perspectives to these challenges — rooted in human dignity, truth, stewardship, and justice.

:::{glossary}
Artificial Intelligence (AI)
  Computer systems capable of performing tasks that typically require human intelligence, including learning, reasoning, problem-solving, perception, and language understanding.

Machine Learning (ML)
  A subset of AI in which systems learn to perform tasks by identifying patterns in data, improving with experience rather than through explicit programming.

Generative AI
  AI systems that create new content (text, images, audio, video, code) based on patterns learned from training data.

Large Language Model (LLM)
  A type of generative AI trained on vast amounts of text data, capable of understanding and generating human-like text. Examples include GPT-4, Claude, and Gemini.

Prompt Engineering
  The practice of designing and refining inputs to AI systems to elicit high-quality, relevant outputs.

Transformer Architecture
  The neural network architecture underlying most modern LLMs, introduced in the 2017 paper "Attention Is All You Need," notable for its attention mechanism.

Supervised Learning
  ML approach where the algorithm learns from labeled data — examples with known correct answers.

Unsupervised Learning
  ML approach where the algorithm discovers patterns in unlabeled data without predefined categories.

Reinforcement Learning
  ML approach where the algorithm learns through trial and error, receiving rewards or penalties for actions.

AI Bias
  Systematic errors in AI outputs that produce unfair results for certain groups, often originating from biased training data or flawed design.

Hallucination
  When an AI system generates confident-sounding but factually incorrect information.

Model Drift
  The degradation of an AI model's performance over time as the data it encounters diverges from its training data.

GDPR
  The General Data Protection Regulation — the European Union's comprehensive data privacy law.

EU AI Act
  The world's first comprehensive AI-specific regulation, classifying AI systems by risk level and imposing corresponding requirements.

Narrow AI
  AI designed for a specific task or narrow set of tasks — all commercially available AI today.

Artificial General Intelligence (AGI)
  Hypothetical AI possessing the full range of human cognitive abilities.
:::

---

## Module 1 Activities

### Quiz: Introduction to AI in Business

:::{exercise} Module 1 Quiz
:label: ex-ch01-quiz

**Answer the following 10 questions based on Chapter 1 content.**

1. **Multiple Choice:** Which of the following best describes the current state of artificial intelligence?
   - (a) AGI has been achieved and is commercially available
   - (b) All commercial AI systems are narrow AI, designed for specific tasks
   - (c) AI systems possess true understanding and consciousness
   - (d) AI has replaced the need for human decision-making in business

2. **True or False:** Generative AI creates new content by truly understanding the meaning of what it produces.

3. **Multiple Choice:** Which type of machine learning would be most appropriate for grouping customers into segments based on purchasing behavior, without predefined categories?
   - (a) Supervised learning
   - (b) Unsupervised learning
   - (c) Reinforcement learning
   - (d) Transfer learning

4. **Short Answer:** Define "prompt engineering" and explain why it is considered a critical business skill in the age of generative AI.

5. **True or False:** The EU AI Act classifies AI systems into risk categories and imposes requirements based on the level of risk.

6. **Multiple Choice:** Amazon's AI recruiting tool demonstrated bias against women primarily because:
   - (a) The algorithm was deliberately programmed to prefer male candidates
   - (b) The training data reflected a decade of male-dominated hiring patterns
   - (c) Women submitted fewer resumes to Amazon
   - (d) The system used gender as an explicit input variable

7. **Short Answer:** Explain the difference between "task displacement" and "job displacement" in the context of AI's impact on the workplace. Provide one example.

8. **True or False:** AI hallucination refers to when an AI system generates confident-sounding but factually incorrect information.

9. **Multiple Choice:** Which component of an effective AI prompt establishes the AI's expertise level and perspective?
   - (a) Context
   - (b) Role
   - (c) Constraints
   - (d) Format

10. **Short Answer:** From a Christian perspective, explain why AI bias is not merely a technical problem but a moral one. Reference at least one Biblical principle in your answer.
:::


### Discussion: The Role of AI in Modern Business

:::{exercise} Module 1 Discussion
:label: ex-ch01-discussion

**Discussion Prompt:**

Consider the following scenario: You are a manager at a mid-sized retail company. Your CEO has just returned from a conference buzzing about AI and wants to "implement AI across the organization" within six months.

**Initial Post (300+ words):**
1. What questions would you ask the CEO before proceeding?
2. Identify three specific business processes in a retail company where AI could create the most value. For each, explain what type of AI would be used and what data would be needed.
3. What are two potential risks the company should consider before rushing to implement AI?
4. How would you apply the principle of Christian stewardship to guide the company's AI adoption strategy?

**Response Posts (150+ words each):**
Respond to at least two classmates. In your responses:
- Build on their ideas with specific examples or alternative perspectives
- Respectfully challenge any assumptions you disagree with
- Connect their points to concepts from the chapter

**Grading Rubric:**
- Depth of analysis and use of chapter concepts (30%)
- Specificity of business process recommendations (25%)
- Thoughtful risk assessment (20%)
- Integration of Christian stewardship principles (15%)
- Quality of peer responses (10%)
:::

### Written Analysis: AI Impact Assessment

:::{exercise} Module 1 Written Analysis
:label: ex-ch01-written-analysis

**Assignment: AI Impact Assessment Report**

Select a company or industry you are interested in and write a 1,000-1,200 word analysis examining how AI is currently being used or could be used to transform business operations.

**Your report must include:**

1. **Company/Industry Overview** (150-200 words)
   - Brief description of the company or industry
   - Current competitive landscape
   - Key business challenges

2. **AI Applications Analysis** (400-500 words)
   - Identify 3-4 specific AI applications relevant to the company/industry
   - For each application, specify:
     - What type of AI is involved (ML, NLP, computer vision, generative AI, etc.)
     - What business problem it addresses
     - What data would be needed
     - Expected business impact (quantify where possible)

3. **Risk and Ethics Assessment** (200-300 words)
   - Privacy implications of the AI applications you described
   - Potential bias concerns
   - Regulatory considerations
   - Impact on employees

4. **Recommendation and Christian Reflection** (200-300 words)
   - Your recommendation for prioritizing AI adoption
   - How Christian business principles should guide implementation
   - One specific ethical guardrail you would put in place

**Format:** APA style, 12-point font, double-spaced, with at least 3 credible sources.

**Grading Rubric:**
| Criteria | Points |
|----------|--------|
| AI Applications Analysis (specificity, accuracy) | 30 |
| Risk and Ethics Assessment (depth, relevance) | 25 |
| Christian Reflection (authenticity, integration) | 20 |
| Writing Quality (clarity, organization, APA) | 15 |
| Sources (quality, proper citation) | 10 |
| **Total** | **100** |
:::

### Reflection: Faith and Technology

:::{exercise} Module 1 Reflection
:label: ex-ch01-reflection

**Faith-Integration Reflection**

:::{epigraph}
"Whatever you do, work at it with all your heart, as working for the Lord, not for human masters."

-- Colossians 3:23 (NIV)
:::

Write a 400-500 word reflection responding to the following prompt:

**God has given humanity the creativity and intelligence to develop artificial intelligence. As a Christian business leader, how do you reconcile the incredible power of AI with the call to humility and stewardship found in Scripture?**

In your reflection, consider:
- What does it mean to be a "steward" of AI technology rather than simply a "user"?
- How does the concept of *Imago Dei* (being made in God's image) inform how we should design AI systems that affect people's lives?
- Proverbs 3:5-6 says, "Trust in the LORD with all your heart and lean not on your own understanding." How does this apply to businesses that are increasingly relying on AI for decision-making?
- Is there a point at which dependence on AI could undermine our trust in God's providence?

**Requirements:**
- Reference at least two specific Scripture passages
- Connect your reflection to at least one concept from Chapter 1
- Be personal and authentic — this is not a research paper
- 400-500 words, submitted as a written document

**Grading:** This reflection is graded on thoughtfulness and authentic engagement with the prompt (not on having "right answers"). Full credit requires genuine wrestling with the tension between technological power and Christian humility.
:::

### Hands-On Activity 1: AI Tool Exploration

:::{exercise} Module 1 Hands-On Activity 1
:label: ex-ch01-activity1

**Activity: Exploring AI Business Tools**

**Objective:** Gain firsthand experience with generative AI tools and evaluate their utility for business applications.

**Instructions:**

:::{dropdown} Part A: Tool Exploration (30 minutes)
:open: true

Choose **two** of the following AI tools to explore:

| Tool | URL | Category |
|------|-----|----------|
| ChatGPT | chat.openai.com | Text generation |
| Google Gemini | gemini.google.com | Multimodal AI |
| Claude | claude.ai | Text generation |
| Perplexity | perplexity.ai | AI search |
| Canva AI | canva.com | Design + AI |
| Copy.ai | copy.ai | Marketing copy |

For each tool:
1. Create a free account (if you don't already have one)
2. Complete at least **three different business tasks**, such as:
   - Write a marketing email for a product launch
   - Create a SWOT analysis for a hypothetical company
   - Generate a customer survey with 10 questions
   - Draft a project timeline for a new initiative
   - Summarize a business article (paste in a real article)
   - Create a job description for a position
3. Save screenshots of your prompts and the AI's responses
:::

:::{dropdown} Part B: Prompt Engineering Practice (20 minutes)
:open: true

Using one of the tools from Part A, complete this prompt engineering challenge:

**Task:** Get the AI to create a professional business proposal for a new coffee shop in your local area.

1. **First attempt:** Write a basic, simple prompt (1-2 sentences). Save the response.
2. **Second attempt:** Apply the prompt engineering techniques from this chapter — include role, context, format, constraints, and specific details. Save the response.
3. **Compare:** Note the differences in quality, specificity, and usefulness between the two responses.
:::

:::{dropdown} Part C: Deliverable
:open: true

Submit a 500-word report that includes:

1. **Tool Comparison Table:**

| Feature | Tool 1: _______ | Tool 2: _______ |
|---------|-----------------|-----------------|
| Ease of use (1-10) | | |
| Output quality (1-10) | | |
| Best business use case | | |
| Biggest limitation | | |
| Free tier usefulness (1-10) | | |

2. **Prompt Engineering Comparison:**
   - Your weak prompt and the AI's response (abbreviated)
   - Your strong prompt and the AI's response (abbreviated)
   - Your analysis of what made the stronger prompt more effective

3. **Reflection:**
   - Which tool would you recommend for a small business owner and why?
   - What surprised you most about working with these tools?
   - What concerns did you have (accuracy, privacy, ethical)?

**Due:** End of Module 1 week
:::
:::

### Hands-On Activity 2: AI Ethics Case Analysis

:::{exercise} Module 1 Hands-On Activity 2
:label: ex-ch01-activity2

**Activity: Building an AI Ethics Decision Framework**

**Objective:** Develop a practical framework for evaluating the ethical implications of AI business applications, grounded in both professional ethics and Christian values.

**Instructions:**

:::{dropdown} Part A: Case Research (20 minutes)
:open: true

Research **one** of the following real-world AI ethics cases:

1. **Clearview AI** — Facial recognition company that scraped billions of social media photos without consent to build a law enforcement surveillance tool.
2. **COMPAS Sentencing Algorithm** — AI system used by U.S. courts to predict recidivism risk, found to have significant racial bias by ProPublica.
3. **TikTok Algorithm** — AI recommendation system accused of creating "filter bubbles" and promoting addictive usage patterns, especially among minors.
4. **Replika AI** — AI companion chatbot that forms emotional relationships with users, raising questions about AI's role in human relationships.

Use at least **two credible sources** for your research.
:::

:::{dropdown} Part B: Framework Development (30 minutes)
:open: true

Create a **one-page AI Ethics Decision Framework** that a business leader could use to evaluate any AI application. Your framework should include:

1. **Five key ethical questions** to ask before deploying an AI system (at least two should be grounded in Christian principles)
2. **A simple scoring rubric** (e.g., Red/Yellow/Green) for each question
3. **Guidance on what to do** if the evaluation reveals concerns

Present your framework as a visual document (table, flowchart, or infographic format).
:::

:::{dropdown} Part C: Case Application (20 minutes)
:open: true

Apply your ethics framework to the case you researched in Part A:

1. Walk through each of your five questions using the real case
2. Assign a score for each question
3. Write a 300-word recommendation: Based on your framework, should this AI application continue as-is, be modified, or be discontinued? What specific changes would you recommend?
:::

:::{dropdown} Part D: Deliverable
:open: true

Submit a document containing:
1. Your AI Ethics Decision Framework (visual format)
2. Your case analysis using the framework
3. Your 300-word recommendation
4. A reference list (APA format)

**Grading Rubric:**
| Criteria | Points |
|----------|--------|
| Framework quality (comprehensive, practical, includes Christian principles) | 35 |
| Case research depth and accuracy | 25 |
| Application of framework to case | 25 |
| Writing quality and presentation | 15 |
| **Total** | **100** |
:::
:::

---

*Chapter 1 has established the foundation for understanding AI in business. In [Chapter 2](#ch02-evolution-deep-learning), we will trace the fascinating history of artificial intelligence — from Alan Turing's revolutionary ideas in the 1950s to the deep learning revolution that powers today's most capable AI systems.*
