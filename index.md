# DSC 180A Methodology Assignment 4

**Name:** Ishaan Tibdewal

**Email:** itibdewal@ucsd.edu

**Section:** D12

**Mentor:** Goutham Valeti

## Quarter 2 Project Brainstorming

**1. What is the most interesting topic covered in your domain this quarter?**

How much memo cleaning matters. In our TF-IDF test, aggressive token filtering deleted key cues like "venmo", "transfer" and "cash" and left some memos empty. Conservative cleaning (normalizing case and spacing, masking long IDs) worked much better.

**2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.**

Use our predicted spending categories as features to predict financial distress (for example, overdrafts or negative balances), and compare logistic regression with XGBoost. If that doesn't work out, I'd fine-tune a small language model to categorize memos directly.

**3. What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**

Measure agreement between labelers before scaling up labeling, and evaluate on a frozen account-level holdout so the same account's memos can't appear in both training and test. I'd also merge overlapping categories (Fast Food vs. Restaurant, Subscriptions vs. Gym) to cut label noise.

**4. What other techniques would you be interested in using in your project?**

FastText with character n-grams (to handle misspelled merchant names), BERT fine-tuning, and local LLMs that suggest labels for active learning. I'd also compare one category's spending trend against FRED macro data.

