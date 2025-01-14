---
id: asr-evaluation
title: Automatic Speech Recognition (ASR) Evaluation
sidebar_label: Automatic Speech Recognition (ASR) Evaluation
---
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

## Automatic Speech Recognition (ASR) Evaluation
This is a simple utility to perform a quick evaluation on the results generated by any Speech to text (STT) or Automatic Speech Recognition (ASR) System.

This utility can calculate following metrics:

* Word Error Rate (WER), which is a most common metric of measuring the performance of a Speech Recognition or Machine translation system

* Levenshtein Distance calculated at word level.

* Number of Word level insertions, deletions and mismatches between the original file and the generated file.

* Number of Phrase level insertions, deletions and mismatches between the original file and the generated file.

* Color Highlighted text Comparison to visualize the differences.

* General Statistics about the original and generated files (bytes, characters, words, new lines etc.)


### Installation

`$ npm install -g speech-recognition-evaluation`

### Usage
Simplest way to run your first evaluation is by simply passing original and generated options to asr-eval command. Where, original is a plain text file containing original transcript to be used as reference; usually this is generated by human beings. And generated is a plain text file containing generated transcript by the STT/ASR system.


`$ asr-eval --original ./original-file.txt --generated ./generated-file.txt`

For more information please visit [this](https://github.com/symblai/speech-recognition-evaluation).
