# LocalPromptBlocker

A Robust Rule-Based Prompt Filtration Tool

 Description

 This Python app provides a flexible and customizable prompt filtration layer for protecting sensitive information and mitigating potential risks associated with large language models (LLMs). It employs a combination of rule-based techniques and sentiment analysis to filter prompts based on various criteria, including:

Personally identifiable information (PII): Phone numbers, email addresses, credit card numbers, social security numbers
Sensitive topics: Violence, drugs, pornography (customizable)
Hate speech: Detected using NLTK's VADER sentiment analyzer
Explicit language: Filtered using a basic pattern-matching approach
Excessive length: Prevents overly long prompts
 Installation

Clone this repository:
Bash
git clone https://github.com/richardaragon/localpromptblocker

content_copy
Install required libraries:
Bash
pip install nltk sklearn

content_copy
Download NLTK resources:
Python
import nltk
nltk.download('punkt')
nltk.download('vader_lexicon')

content_copy
 Usage

Import the filter_prompts function:
Python
from local_prompt_blocker import filter_prompts
Use code with caution. Learn more
content_copy
Pass a prompt to the function:
Python
result = filter_prompts("Your prompt text here")
print(result)
Use code with caution. Learn more
content_copy
 Customization

Adjust thresholds, word lists, and patterns in the filter_prompts function to align with your specific requirements.
Train a machine learning model using libraries like scikit-learn for more advanced filtering capabilities.
 License

 This project is licensed under the MIT License. See the LICENSE file for details.

 Contributing

 We welcome contributions! Please feel free to submit pull requests or open issues for feature requests or bug reports.
