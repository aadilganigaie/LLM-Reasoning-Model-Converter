# LLM-Reasoning-Model-Converter

This repository contains a Jupyter Notebook that transforms any Large Language Model (LLM) Mistral 7B in our case into a reasoning—or “self-thinking”—model by leveraging Unsloth, GRPO (Group Relative Policy Optimization), and RLHF (Reinforcement Learning from Human Feedback).

# Overview
The provided notebook demonstrates a novel fine-tuning approach that:

Converts Standard LLMs: Augments any base model with reasoning capabilities by automatically generating chain-of-thought tokens.
Optimizes VRAM Usage: Uses Unsloth’s efficient fine-tuning techniques to reduce memory overhead.
Reinforces Self-Verification: Applies GRPO to compare groups of generated responses, reinforcing those that better satisfy a custom reward function, with additional alignment via RLHF.
This integrated approach enables the model to “think” more deeply and verify its own outputs, thereby improving performance on complex reasoning tasks.

# Features
Plug-and-Play Conversion: Easily convert your favorite LLM into a reasoning model.
Efficient Training: Leverage Unsloth to minimize VRAM requirements and training costs.
Customizable RLHF Pipeline: Modify reward functions and fine-tuning settings to suit specific domains or tasks.
Requirements
Python 3.12 or higher
Jupyter Notebook or JupyterLab
Unsloth
TRL (for GRPO and RLHF support)
