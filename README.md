# Traffic Light Controller in Verilog

This project implements a traffic light controller system in Verilog, simulating a traffic light system with a main highway and a country road. The system transitions through different states based on the presence of a car on the country road.

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The traffic light controller is designed to manage the traffic signals at an intersection where a main highway and a country road meet. The system uses a finite state machine (FSM) to transition between different states of traffic lights based on the presence of a car on the country road.

## Project Structure

The project consists of the following main modules:

- `stimulus`: This module generates the clock and clear signals and applies test stimuli to the `sig_control` module.
- `sig_control`: This module implements the FSM to control the traffic signals.

### State Definitions

- `S0`: Main highway GREEN, country road RED
- `S1`: Main highway YELLOW, country road RED
- `S2`: Main highway RED, country road RED
- `S3`: Main highway RED, country road GREEN
- `S4`: Main highway RED, country road YELLOW

### Delays

- `Y2RDELAY`: Yellow to Red delay (3 clock cycles)
- `R2GDELAY`: Red to Green delay (2 clock cycles)

## Getting Started

### Prerequisites

To simulate and test the Verilog code, you will need a Verilog simulator such as:

- ModelSim
- Icarus Verilog
- Xilinx Vivado

### Cloning the Repository

```bash
git clone https://github.com/girija2103/Traffic-Signal-Controller-Verilog.git
cd Traffic-Signal-Controller-Verilog
