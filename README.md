# Two-Stage Loan Approval Prediction

## Overview

This project implements a two-stage machine learning pipeline for loan approval analysis.

The system first predicts whether a loan application is likely to be approved and, for approved applicants, predicts the expected loan amount.

## Problem Statement

Loan approval involves evaluating an applicant's financial and personal attributes to determine eligibility. This project uses machine learning to:

- Predict loan approval status.
- Predict the loan amount for approved applicants.
- Identify the key factors influencing model predictions using SHAP explainability.

## Project Workflow

```text
Applicant Information
        │
        ▼
Stage 1: Classification
        │
   ┌────┴────┐
   │         │
Rejected   Approved
             │
             ▼
      Stage 2: Regression
             │
             ▼
    Predicted Loan Amount