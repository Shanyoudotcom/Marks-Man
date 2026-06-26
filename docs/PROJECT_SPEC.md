# PROJECT_SPEC.md

# Marks Man

**Version:** 1.0 (Foundation)

---

# Vision

Marks Man is an AI-powered examination intelligence platform designed to help medical students study more efficiently by forecasting examination topics using historical evidence, curriculum analysis, educational resources, and machine learning.

Marks Man is **not** an answer bank.

Marks Man is **not** a question bank.

Marks Man is an **Exam Intelligence Platform**.

Every recommendation made by the system should be explainable using objective evidence.

---

# Mission

Develop the world's most accurate and transparent examination prediction engine.

The platform should answer questions such as:

* What is most likely to appear in the next examination?
* Why is it likely?
* How confident is the prediction?
* How should I study it?
* Which resources should I use?
* What is the expected return on my study time?

---

# MVP (Minimum Viable Product)

University

RGUHS

Curriculum

CBME RS4 / RS5

Subjects

* Community Medicine
* Forensic Medicine

Outputs

* Predicted Long Essays
* Predicted Short Essays
* Predicted Short Answers
* Predicted MCQs

---

# Long-Term Goal

Marks Man should eventually support

* All MBBS subjects
* All Indian universities
* NEET PG
* INI-CET
* FMGE
* USMLE
* PLAB

The architecture must therefore be completely modular.

No component should assume RGUHS-specific behaviour.

---

# Core Principles

## 1. Explainability

Every prediction must explain itself.

Example

Tuberculosis

Probability

96%

Evidence

Historical recurrence

Gap analysis

CBME importance

Teaching emphasis

Guideline updates

No black-box predictions.

---

## 2. Evidence First

Predictions must be based on measurable evidence.

Evidence includes

* Historical university papers
* Companion recurrence
* CBME competencies
* Official curriculum
* Teaching hours
* DBMCI emphasis
* Marrow question density
* National guideline updates

---

## 3. Separation of Data and Logic

Raw data must never be modified.

The system should separate

Raw Data

↓

Normalized Data

↓

Features

↓

Predictions

↓

Frontend

This allows improvements to the prediction engine without changing historical datasets.

---

## 4. Version Everything

Every

Dataset

Prediction Model

Algorithm

Guideline

Question Paper

Companion Edition

must be versioned.

Nothing should ever be overwritten.

---

## 5. Scalability

The system should support

multiple

Universities

Subjects

Curricula

Textbooks

Prediction models

without requiring architectural redesign.

---

# Data Sources

Primary

Companion

Historical question papers

CBME

RGUHS Ordinance

DBMCI

Marrow

Secondary

Park

PVD Shetty

Reddy

Biswas

National Guidelines

---

# Prediction Philosophy

Predictions are generated from multiple independent evidence sources.

No single source determines the final score.

Current weighting

Historical recurrence

CBME importance

Teaching emphasis

Guideline updates

Question density

Gap analysis

Rotation analysis

The weighting system should be configurable.

---

# Knowledge Representation

Questions should never exist as isolated entities.

Every question belongs to

Subject

↓

Chapter

↓

Master Topic

↓

Subtopic

↓

Question Variant

Example

Screening

↓

Validity

↓

Sensitivity

↓

Specificity

↓

Predictive Value

↓

Lead Time Bias

Historical questions reference these concepts rather than duplicating information.

---

# Explainable AI

Every prediction card shown to the user must contain

Probability

Confidence

Historical appearances

Reasons

Supporting evidence

Recommended resources

Expected marks

Estimated study time

Revision priority

---

# Study Optimizer

Marks Man should generate personalized study plans.

Inputs

Exam Date

Study Hours

Completed Topics

Weak Areas

Outputs

Daily Study Plan

Revision Calendar

Expected Coverage

Marks per Hour

---

# Development Philosophy

Marks Man should be built like a production software product.

Not as a collection of scripts.

Every architectural decision should be documented.

Every feature should be tested.

Every prediction should be reproducible.

---

# Repository Structure

The repository should remain organized as

/docs

Research

Specifications

Architecture

Database

Algorithms

/data

Raw datasets

Never modified

/backend

Prediction engine

API

/frontend

User interface

/research

Experiments

Statistical analyses

Validation studies

/tests

Unit tests

Integration tests

Validation tests

---

# Engineering Rules

Do not hardcode universities.

Do not hardcode subjects.

Do not hardcode prediction weights.

Do not modify imported datasets.

Keep prediction algorithms modular.

Document every architectural decision.

Write readable code before clever code.

Optimise only after profiling.

---

# Success Criteria

Version 1 succeeds if it can

Import data.

Normalize topics.

Generate explainable predictions.

Recommend study plans.

Validate predictions against historical papers.

---

# Definition of Done

A feature is complete only when

It works.

It is tested.

It is documented.

It is explainable.

It does not reduce maintainability.

---

# Motto

> Study smarter. Predict better. Learn with evidence.

