# Word Count with Hadoop MapReduce

This repository demonstrates a simple **Word Count** program using **Hadoop MapReduce**. The goal of this program is to read a large corpus of text data, count the occurrences of each word, and display the word counts.

# Overview

The **WordCount** example is a classic MapReduce program that reads a text file and counts how many times each word appears in the input dataset.

### How it works:
1. **Mapper**: The mapper tokenizes the input text into words and outputs key-value pairs (`word, 1`).
2. **Reducer**: The reducer aggregates the word counts and sums them up for each word.
3. **Output**: The final output is a list of words along with their corresponding counts.

The program consists of the following components:
- **WordCount_Mapper.java**: Mapper class that emits word counts.
- **WordCount_Reducer.java**: Reducer class that aggregates the counts and outputs the final results.
- **WordCount_Runner.java**: Driver class that sets up the Hadoop job.

## Prerequisites

Before running this program, make sure you have the following tools installed:

1. **Hadoop**: The program uses Hadoop MapReduce, so you need to have Hadoop installed on your system. Follow the [My Own Video Guideline on How to Install Hadoop](https://youtu.be/kUX6dCbdU3Q).
   
2. **Java Development Kit (JDK)**: The program is written in Java, so make sure you have JDK installed. You can download it from [here](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html).

3. **Maven**: This project uses Maven for dependency management. You can install it from [here](https://maven.apache.org/install.html).

## How to Run

### 1. Clone the repository:

```bash
git clone https://github.com/Kundan-Rwanda/WordCount.git
cd WordCount
