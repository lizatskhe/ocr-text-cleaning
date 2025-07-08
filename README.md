# OCR Text Cleaning

This project focuses on cleaning OCR-generated text and evaluating the quality of cleaned outputs using both human-annotated scores and automatic evaluation metrics. It includes preprocessing, alignment of OCR vs. cleaned text, and comparative analysis using models like LLaMA and Phi-3.

## Project Overview

Optical Character Recognition (OCR) systems often produce noisy or incomplete outputs. In this project I:

- Clean OCR-generated text using simple heuristics.

- Align noisy-clean sentence pairs.

- Score the quality of cleaned text using ROUGE and LLM-based judges.

- Collect human judgments and analyze correlation with automatic scores.

## Project Structure

`ocr_cleaning.ipynb` - Main notebook for OCR text cleaning, alignment, and evaluation

`the_vampyre_ocr_5k.json` - Subset of the OCR dataset (first 5,000 tokens)

`aligned_sentences_with_scores\aligned_sentences.json` - Aligned noisy and cleaned sentence pairs from OCR data

`aligned_sentences_with_scores\aligned_sentences_with_rouge.json` - Sentence pairs with ROUGE metric scores for quality assessment

`aligned_sentences_with_scores\aligned_sentences_with_human_scores.json` - Sentence pairs annotated with human evaluation scores

`eval_results\correlation_results.json` - Correlations between automated metrics and human scores

`eval_results\ocr-judge.json` - LLM evaluations

`eval_results\ocr-llama.json` - Cleaned text by Llama

`eval_results\ocr-phi3.json` - Cleaned text by Phi3

## Evaluation

- ROUGE – Automated n-gram overlap score.

- LLaMA & Phi-3 – Alternative LLM scorers.

- Human Evaluation – Manual scores to compare with automated methods.
