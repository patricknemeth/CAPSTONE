# Exploring Roleplaying Game Player Behavior and Its Impact on Narrative Experiences in Interactive Media¶

## project overview
This project focuses on understanding how player choices and behaviors in role-playing games impact narrative branching and story outcomes. I will explore roleplaying game player behavior and its impact on narrative experiences in video games and other interactive media, as well as attempt to understand the diverse ways in which users engage with narrative content.

#### The User: 

This project addresses challenges faced by game developers, designers,
and storytellers across various digital media. It also holds potential benefits for
consumers, offering more personalized and immersive experiences in interactive
entertainment that can adapt to individual behaviors and choices.

#### The Big Idea: 
Machine learning will be utilized to analyze player behavior data,
employing techniques like clustering for player segmentation and predictive modeling to
anticipate player actions, and Natural Language Processing can extract player
sentiment, preferences, and emotions from text documents. These techniques focus on
extracting meaningful insights from player data, which can inform both narrative and
gameplay design.

#### The Impact: 
The project aims to elevate narrative engagement in videogames and
other forms of interactive media utilizing machine learning and AI, which could
potentially increase consumer satisfaction and retention. Integrating data-driven insights
with adaptive storytelling techniques could significantly contribute to both the gaming
industry as well as broader digital narrative experiences as a whole.


## Dataset

Split into two files (one for character descriptions and one for narrative posts), the "Deep Dungeons and Dragons Corpus" (DDDC) contains an extensive collection of narrative posts and character descriptions from various pen and paper role-playing games collected from roleplayerguild.com.  This dataset includes 56,555 entries across 1,544 unique threads, each detailed with post sequences, author information, and narrative content. It presents a terrific opportunity for exploratory data analysis and natural language processing.

### Data Dictionary

### DDDC.txt

| Field             | Description |
|-------------------|-------------|
| `thread_id`       | Numeric identifier for each story thread. Posts sharing the same `thread_id` are part of the same narrative thread. |
| `post_id`         | Unique identifier for each post within a thread, starting from 0. The ascending order represents the chronological sequence of the narrative. |
| `web_id`          | Post ID on the roleplayerguild.com website, used primarily for data collection purposes. |
| `author_name`     | Name of the contributor of the post. This field allows tracking of posts by the same author across different threads and links to character descriptions. |
| `author_join_time`| The time when the author joined the roleplayerguild.com website. This column is not actively used in the analysis. |
| `author_num_posts`| Total number of posts made by the author on the website. Like `author_join_time`, this column is not central to the narrative analysis. |
| `post_text`       | The actual content of the post, containing action descriptions and forming the core of the narrative data. |


### DDDC.txt.charinfo 

| Field         | Description |
|---------------|-------------|
| `thread_id`   | Numeric identifier corresponding to the thread ID in DDDC.txt. |
| `author_name` | Author's name, linking the character descriptions to their respective posts in DDDC.txt. |
| `dummy`       | A field to be ignored. |
| `char_description` | The detailed description of the character written by the author. |


## Project Updates - Sprint 2

### Preprocessing Steps:
- Cleaned dataset: Dropped unnecessary columns and managed missing values.
- Text preprocessing: URLs removed, text normalized to lowercase, and cleaned of special characters.
- Feature Engineering: Derived post length and sentiment analysis.

### EDA Highlights:
- Author activity analysis: Detailed insights into posting behavior and engagement within the community.
- Post lengths investigation: Explored the narrative depth across posts.
- `post_text` complexity: Highlighted the diversity of narrative contributions.

### Towards Advanced Modeling:
- Set the foundation for baseline modeling, focusing on sentiment analysis and Named Entity Recognition (NER).
- Prepared the data for advanced analysis techniques

