# ElecBench: A Power Dispatch Evaluation Benchmark for Large Language Models

This repository contains the test datasets used in the paper "ElecBench: A Power Dispatch Evaluation Benchmark for Large Language Models".

## Introduction

In response to the urgent demand for grid stability and the complex challenges posed by renewable energy integration and electricity market dynamics, the power sector increasingly seeks innovative technological solutions. Large Language Models (LLMs) have emerged as a key technology to improve efficiency and promote intelligent progress in the power sector with their excellent natural language processing, logical reasoning, and generalization capabilities. 

However, the absence of a performance evaluation benchmark for LLMs in the power sector has limited the effective application of these technologies. Addressing this gap, our study introduces "ElecBench", an evaluation benchmark for LLMs within the power sector.

## Dataset Overview

This repository includes the following test datasets:

1. **General Test Set**
2. **Monitoring Test Set**
3. **Dispatch Test Set**
4. **Blackstart Test Set**

Each test set is provided in `.jsonl` format and includes various scenarios designed to evaluate the performance of LLMs on core metrics such as factuality, logicality, stability, security, fairness, and expressiveness.

## File Descriptions

- `general.jsonl`: Test set for general scenarios.
- `monitoring.jsonl`: Test set for monitoring scenarios.
- `dispatch.jsonl`: Test set for dispatch scenarios.
- `blackstart.jsonl`: Test set for blackstart scenarios.

## Partial Open Source

This repository is partially open source. It includes selected test datasets used in our study to enable the research community to evaluate and improve LLM performance in the power sector.

## How to Use

1. **Reading the Data**: Each `.jsonl` file contains records in JSON Lines format, where each line is a separate JSON object. You can read these files using Python or any other programming language that supports JSON parsing.

   Example in Python:
   ```python
   import json

   def read_jsonl(file_path):
       with open(file_path, 'r', encoding='utf-8') as file:
           for line in file:
               data = json.loads(line.strip())
               print(data)

   # Read the general test set
   read_jsonl('general.jsonl')
