# GPT Job Application Assistant

(Note this is still a work in progress)

## Overview

The GPT Job Application Assistant is a Python application designed to help automate job applications by generating tailored cover letters and job applications based on provided prompts. The application utilizes the OpenAI's gpt-3.5-turbo or gpt-4 API to process the prompts and generate appropriate responses.

### Features

- Read prompts from text files (prompt.txt, resume.txt, job_listing.txt)
- Process prompts with gpt-3.5-turbo or gpt-4 API
- Generate a tailored cover letter
- Save generated content to a text file (output.txt) without overwriting previous content
- Calculate and display the cost and tokens used for each generated cover letter

## Installation

### Pre-requisites

Python 3.11 or higher
Poetry 1.4.2 or higher

### Setup

1. Clone the repository and navigate to the project directory

```
git clone git@github.com:sdevgill/gpt-jobs.git
cd gpt-jobs
```

2. Install Poetry if you haven't already

```
curl -sSL https://install.python-poetry.org | python3 -
```

3. Install the required packages with poetry

```
poetry install
```

4. Activate the virtual environment created by Poetry

```
poetry shell
```

5. Create a .env file for the OpenAI API key and set it to your API key

```
cp .env.example .env
```

6. Write to the input text files with the appropriate content

```
prompt.txt: General prompt instructions for the cover letter (already written, edit it to your liking if wanted)
resume.txt: Your resume text
job_listing.txt: The job listing text
```

### Usage

1. Run the application

```
python app.py
```

## License

This project is licensed under the MIT License. See the LICENSE file for details.
