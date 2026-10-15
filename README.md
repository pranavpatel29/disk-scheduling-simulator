# Disk Scheduling Simulator — SCAN, C-SCAN and Research-Inspired Heuristic

## Project Overview

The Disk Scheduling Simulator is an Operating Systems SLA Review 2 project that demonstrates how disk scheduling algorithms organize disk requests and calculate total disk-head movement.

The project provides an interactive web interface where users can enter disk configuration details, run simulations, view head movement diagrams, and compare algorithm results.

## Live Demo

**Website:** https://pranavpatel29.github.io/disk-scheduling-simulator/

**GitHub Repository:** https://github.com/pranavpatel29/disk-scheduling-simulator

## Features

- Enter the total number of disk tracks.
- Set the initial disk-head position.
- Enter a custom disk request queue.
- Select the initial direction for SCAN and C-SCAN.
- View request service order and disk-head path.
- Calculate total head movement and average movement per request.
- View graphical movement diagrams.
- Expand step-by-step movement calculations.
- Compare SCAN, C-SCAN, and an experimental research-inspired heuristic.
- Validate input and display errors for invalid track values.

## Algorithms Implemented

### 1. SCAN Disk Scheduling

The disk head moves in the selected direction, services requests along the way, reaches the relevant disk end, and then reverses direction to service remaining requests.

### 2. C-SCAN Disk Scheduling

The disk head services requests in one direction. After reaching the disk end, it returns to the opposite end and continues servicing requests in the same direction.

### 3. Research-Inspired Neighbour Heuristic

This experimental classroom implementation is inspired by the neighbour-selection and disk-end-distance idea discussed in the research paper by Elnaas and Sullabi (2024). The later path-building steps are interpreted for this simulator, so the implementation is not claimed to be an exact reproduction of the complete published algorithm.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- SVG for movement diagrams
- GitHub for source-code hosting
- GitHub Pages for website deployment

## How to Use

1. Open the live demo.
2. Enter the total number of tracks.
3. Enter the initial head position.
4. Enter the disk request queue using comma-separated track numbers.
5. Choose the initial directions for SCAN and C-SCAN.
6. Click **Run Both Algorithms**.
7. Compare the service orders, total head movements, diagrams, and calculation tables.

## Project Team

- **Pranav Patel** — Roll No. 40
- **Ketan Patil** — Roll No. 41

## Research Reference

Elnaas and Sullabi, *Proposing Disk Scheduling Algorithm to Enhance the Efficiency of Disk Performance*, International Journal of Engineering and Information Technology (IJEIT), Volume 12, Number 1, December 2024.

[Read the research paper](https://ijeit.misuratau.edu.ly/index.php/ijeit/article/download/485/378)

## Academic Purpose

This project was developed for Operating Systems SLA Review 2 to demonstrate disk scheduling concepts, implementation, movement calculations, graphical visualization, and performance comparison.

**Note:** Simulation results depend on the disk configuration, request queue, and selected direction. The experimental heuristic should be treated as an educational interpretation rather than a verified implementation of the complete research algorithm.
