# Kernel — Low-Level Systems & Qwen3 GRPO Fine-Tuning

## Overview
The `kernel` repository contains low-level x86 assembly bootloader scripts and the Qwen3-4B Group Relative Policy Optimization (GRPO) fine-tuning Jupyter notebook (`nb/Qwen3_(4B)-GRPO.ipynb`).

## Architecture & Pipeline
- **GRPO Fine-Tuning Notebook (`nb/Qwen3_(4B)-GRPO.ipynb`)**: Implements parameter-efficient fine-tuning of Qwen3 using Unsloth, Hugging Face TRL, SFT pre-finetuning, and GRPO reinforcement learning.
- **Assembly Bootloaders**: Low-level x86 boot sector print and simple bootloader programs (`boot_sect_print.asm`, `boot_sect_simple.asm`).

## Data
- **Dataset**: OpenR1 Math dataset and Open Math Reasoning dataset for LLM alignment.

## Method & Algorithms
- **GRPO Reinforcement Learning**: Optimizes language model reasoning traces without a separate value critic network.
- **Low-Level Assembly**: Direct x86 BIOS real-mode execution routines.

## Verified Results & Metrics
- Successfully set up SFT pre-finetuning for prompt formatting followed by GRPO reward-based reinforcement learning loops on Qwen3 models.

## Limitations & Caveats
- Educational low-level assembly scripts and experimental LLM reasoning notebook.

## Run Instructions
```bash
# To run the LLM reasoning notebook:
jupyter notebook nb/Qwen3_(4B)-GRPO.ipynb
```

## CV Bullet Points
- Implemented reinforcement learning fine-tuning pipelines (GRPO) on Qwen3-4B using Unsloth and Hugging Face TRL to train reasoning models.
- Developed low-level x86 assembly bootloader programs demonstrating fundamentals of system startup and real-mode execution.

## Claims to Avoid
- Do not claim enterprise operating system development or large-scale model pre-training.
