# Improving Supply Chain Resilience under Partial Visibility

## Overview

This project presents a computational study of supply chain resilience under partial network visibility.

The model considers a focal firm that observes only part of a multi-tier supplier network and has a limited resilience budget. The firm can allocate resources to two types of local interventions: expanding upstream visibility through monitoring and assigning backup sourcing to selected tier-1 suppliers.

## Research Questions

The project addresses three questions:

1. How much can a focal firm reduce disruption exposure with a fixed resilience budget?
2. Does the relative value of visibility and backup sourcing depend on network topology?
3. Do structurally targeted interventions outperform random allocation of the same resources?

## Model

The supply network is represented as a directed layered graph with three upstream supplier tiers and one focal firm. Edges run from supplier to customer.

Three stylized network topologies are considered:

- Sparse networks
- Dense networks
- Hub-dominated networks

The analysis compares targeted and random policies under the same resilience budget.

## Policies

The following policies are evaluated:

- Baseline: no additional intervention
- Visibility only: monitoring selected upstream nodes
- Backup only: assigning backup sourcing to selected tier-1 suppliers
- Hybrid: combining visibility and backup sourcing
- Random visibility, random backup, and random hybrid benchmarks

## Metrics

The main outcome is the share of impacted tier-1 suppliers under simulated disruption scenarios.

Additional metrics include:

- Probability of severe disruption
- 90th percentile of disruption impact
- Average disruption impact across network topologies

## Key Findings

- Resilience investments are topology-dependent.
- In sparse networks, targeted backup sourcing performs best.
- In dense and hub-dominated networks, targeted visibility produces the largest reduction in disruption exposure.
- Structurally targeted policies outperform random allocation of the same resources.
- Visibility and backup sourcing operate through different resilience mechanisms.

## Report

The full project report is available here:

[supply_chain_resilience_report.pdf](supply_chain_resilience_report.pdf)

## Repository Structure

```text
supply_chain_resilience.ipynb       Jupyter notebook with the computational experiment
supply_chain_resilience_report.pdf  Project report
requirements.txt                    Python dependencies
README.md                           Project description
