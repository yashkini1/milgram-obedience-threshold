# milgram-obedience-threshold
Interactive visualization for AP Psychology Case Project
# Obedience Threshold

An interactive computational visualization of Stanley Milgram's behavioral study of obedience.

## About

This project reconstructs the progression of all 40 participants through Milgram's 30-level shock generator, from 15 V to 450 V. Rather than displaying the study's final result as a static graph, the program models obedience as a changing population: participants leave the visualization at the voltage level where they refused to continue.

The visualization dynamically computes:

- Number of participants continuing
- Number of participants who refused
- Percentage of participants still obeying
- Participant attrition across increasing voltage levels
- An obedience survival curve

It also incorporates qualitative elements of the study, including the learner's responses and the experimenter's standardized verbal prods.

## Data

The visualization is based on the results reported in Table 1 of the assigned case study, *Obey at Any Cost?*, which discusses Stanley Milgram's behavioral study of obedience.

Of the 40 participants:

| Voltage | Participants Who Refused |
|--------:|-------------------------:|
| 300 V | 5 |
| 315 V | 4 |
| 330 V | 2 |
| 345 V | 1 |
| 360 V | 1 |
| 390 V | 1 |

No participants refused before 300 V. The remaining 26 participants (65%) reached the maximum 450 V level.

## How It Works

Each figure represents one participant. The program assigns anonymous participant IDs to the aggregate refusal counts reported in the study. As the simulated voltage increases, participants whose refusal threshold has been reached leave the active population.

The program then recalculates the obedience rate and constructs the survival curve in real time.

The participant IDs are only visual representations; the original data reports aggregate counts rather than individual participant identities.

## Purpose

The goal is to represent both the quantitative results and the psychological concept of obedience to authority in a form that would be difficult to communicate through a static graph alone.

## Running Locally

Download the repository and open `index.html` in any modern web browser. No external libraries or installation are required.

## Technologies

- HTML
- CSS
- JavaScript
- HTML Canvas