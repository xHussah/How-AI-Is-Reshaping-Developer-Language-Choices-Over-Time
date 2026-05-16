# How AI Is Reshaping Developer Language Choices Over Time

This project investigates whether the rise of large language models, specifically the release of ChatGPT in November 2022 influenced programming language preferences in open-source AI development. Using metadata collected from almost 5,750 AI-related GitHub repositories spanning 2020–2025, the study tracks shifts in language popularity, repository engagement, and ecosystem composition before and after ChatGPT's release.

## Key findings 
Python's share among new AI repositories declined from 47.86% to 40.41% post-ChatGPT, while the average stars received by Python repositories surged by 168% (from 2,171 to 5,812), indicating a shift from Python as the default language to Python as the high-impact platform for LLM projects.

## Dataset
Data was collected via the GitHub REST API, targeting the top-starred AI-related repositories from 2020 to 2025 (250 per quarter per year, almost 1,000 per year).

**Features collected per repository:** name, owner, URL, description, stars, forks, creation date, last push date, primary language, all languages (bytes), topics, contributors count.

**Total observations:** approx. 5,750 repositories.

## Technologies Used
**Language:**
- Python

**Platform:**
- Google Colab

## Developers
- Afnan Alkharji
- Deema Alfarhoud
- Hussah Alotaibi
- Falwa Alkhalifah
- Sana Alotaibi

This project was completed in November 2025. 
