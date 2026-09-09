---
layout: page
title: Registration
permalink: /registration.html
---

# Project Registration (Setup Only)

This is an individual project. Please create accounts on Kaggle, GitHub, Weights & Biases, and Hugging Face if you haven't already.

📽️ Registration walkthrough slides: [Click here]({{ site.data.term.registration_slides_url }})

## 1. Kaggle Competition Setup

1. Join the Kaggle competition using [this link]({{ site.data.term.kaggle_competition_link }}).
2. After joining, go to the **Code** tab and create a new notebook.
3. Name your notebook: `DL-YourRollNo-notebook-{{ site.data.term.term_code }}`
   Example: `DL-21f1001234-notebook-{{ site.data.term.term_code }}`
4. Share the notebook with the competition admin: **`{{ site.data.term.kaggle_admin_username }}`** (view access is enough — keep it private).
5. Make at least one baseline submission (even a dummy model is fine).

> **Note:** Later, you may complete training separately in Kaggle or Colab, then upload the trained models to Kaggle Hub and import them into your inference notebooks when submitting.

## 2. GitHub Repo Setup

1. Create a repository for your project — **private, with instructor access**.
2. Add a basic `README.md` containing:
   - Project title (tentative)
   - Your name & ID
   - Empty folder structure (e.g., `/scripts`, `/notebooks`, `/data`)
3. You'll add actual code and notebooks later during the project.

📁 Sample GitHub repo structure & guideline: [Click here]({{ site.data.term.sample_repo_structure_url }})

## 3. Weights & Biases (W&B) Setup

Create a new W&B project named: `YourRollNo-{{ site.data.term.term_code }}`

## Final Step

Once all three setups above are done, submit the [Registration Form]({{ site.data.term.registration_form_url }}) with your Kaggle username, GitHub repo link, and W&B project URL.

> ⚠️ **Without completing all three setups (Kaggle, GitHub, W&B), submitting at least 2 milestones, and submitting Form 1, you will not be eligible for evaluation or viva.**
