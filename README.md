LLM Red Teaming & Adversarial Evaluation Suite

This repository contains a comprehensive corpus of Large Language Model (LLM) attack vectors and a Python test harness to evaluate model robustness. It covers techniques ranging from basic prompt injection to advanced cryptographic and mathematical exploits (GCG).

Files

attack_corpus.jsonl: A JSON Lines dataset containing over 60 distinct attack vectors (English).

attack_corpus_thai.json: A JSON dataset containing 75 attack vectors adapted for Thai language context.

red_team_runner.py: The main evaluation script for English attacks.

red_team_runner_thai.py: The evaluation script specialized for Thai language nuances.

indirect_red_team.py: Simulates indirect injection via email/documents.

defense_runner.py: Implements the "Sandwich Defense" pattern.

Usage

Install Dependencies:

pip install openai


Set API Key:
Export your OpenAI API key as an environment variable:

export OPENAI_API_KEY='sk-...'


Run the Evaluation:

python red_team_runner.py       # English
python red_team_runner_thai.py  # Thai


Analyze Results:
Check the generated .csv files for Pass/Fail assessments.

Disclaimer

This dataset and code are provided for educational and security research purposes only. They are intended to help developers identify weaknesses in their own systems to improve safety.
