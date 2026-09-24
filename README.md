# LUB 2 — Saudi Arabic Semantic Understanding & Customer Care Shield

## Overview

LUB 2 is an AI platform designed to understand Saudi Arabic text beyond its literal meaning, with a particular focus on customer-service contexts.

The project aims to detect hidden complaints, sarcasm, sentiment, polarity, customer-service relevance, and escalation risk by considering both the message and its context.

The system uses Arabic pretrained language models that are fine-tuned on project-specific Saudi Arabic data to improve contextual understanding.

---

## Dataset

The `LUB-Saudi-Arabic-Intent.csv` dataset was created for the LUB 2 project to support research and experimentation in Saudi Arabic contextual understanding.

The dataset contains **1,500 examples** covering different Saudi Arabic expressions and customer-service scenarios.

Each example includes the original text, contextual information, semantic annotations, and classification labels used for model training and evaluation.

### Main Tasks

The dataset supports multiple NLP classification tasks, including:

- Complaint Detection
- Sarcasm Detection
- Surface Polarity Classification
- Intended Polarity Classification
- Customer Service Classification
- Escalation Risk Classification
- Intent Type Classification
- Emotion Classification

---

## Dataset Features

The dataset contains information such as:

- `ID` — Unique example identifier
- `Text` — Saudi Arabic text
- `Region` — Saudi dialect/region
- `Context` — Context surrounding the message
- `Surface_Meaning` — Literal meaning
- `Intended_Meaning` — Intended meaning
- `Intent_Type` — Type of user intent
- `Emotion` — Detected emotion
- `Emotion_Intensity` — Emotion intensity
- `Sarcasm` — Sarcasm label
- `Sarcasm_Intensity` — Sarcasm intensity
- `Polarity_Surface` — Surface-level polarity
- `Polarity_Intent` — Intended polarity
- `Relation` — Semantic relation
- `Customer_Service` — Customer-service relevance
- `Complaint` — Complaint label
- `Escalation_Risk` — Escalation risk level
- `Explanation` — Explanation of the annotation
- `Source` — Dataset source/version information

---

## Example

A message may appear positive on the surface while expressing a negative intention.

**Text:**

> يعطيكم العافية، دفعت رسوم الاشتراك السنوي وبعدها ألغيتوا الخدمة وما رجع لي المبلغ.

**Context:**

> العميل تواصل مع خدمة العملاء بخصوص اشتراك سنوي تم إلغاؤه، وكان يتابع موضوع استرجاع المبلغ.

This type of example demonstrates the project's focus on understanding the difference between surface wording and the actual intended meaning.

---

## Model

LUB 2 uses **MARBERTv2**, an Arabic pretrained language model, which was fine-tuned on the LUB 2 dataset for multiple classification tasks.

The models use:

**Text + Context**

as the primary input to improve contextual understanding.

The data was divided into training, validation, and testing sets to evaluate model performance.

---

## Project Goal

The main goal of LUB 2 is to contribute to better Arabic and Saudi Arabic language understanding in real-world customer-service environments.

The project can support applications such as:

- Customer support centers
- Telecommunications
- E-commerce
- Banking
- Government services
- Delivery and transportation
- Digital customer-service platforms

---

## License

This dataset is intended for research and experimentation as part of the LUB 2 project.
