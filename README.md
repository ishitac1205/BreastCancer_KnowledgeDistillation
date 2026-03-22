
# Breast Cancer Classification using Knowledge Distillation

This project explores how knowledge distillation can be used to compress a high-performing model into a smaller, more efficient one for medical image classification.

## Problem

High-accuracy models are often large and expensive to deploy.
The goal here is to retain performance while reducing model size.

## Approach

1. Train a high-capacity **teacher model**
2. Train a smaller **student model** using:

   * ground truth labels
   * soft targets from the teacher
3. Combine both signals using a distillation loss

## Training Setup

* Teacher model trained to high accuracy (~98%)
* Student model trained using distillation (~96%)
* Focus on balancing performance vs efficiency

## Why this matters

In real-world medical systems, models often need to run on limited hardware.
Distillation allows deployment without a major drop in accuracy.

## Tech Stack

* PyTorch
* CNN architectures
* Knowledge distillation loss functions

## Key Takeaway

A properly trained student model can achieve near-teacher performance while being significantly lighter.

## Status

Research-oriented project exploring model compression techniques.
