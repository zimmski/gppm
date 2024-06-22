# gppm
GPU Power and Performance Manager

**Status:** Alpha

gppm is an aimed to be used with llama.cpp and NVIDIA P40 GPUs. Currently llama.cpp doesn't provide functionality to reduce the power consumption of P40s in idle mode. This is where gppm jumps in. gppm monitors llama.cpp's output und accordingly changes the performance modes of installed P40s. gppm is in its alpha phase, meaning it is in active development and not yet feature-complete. I welcome feedback and contributions.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)

## Installation

To get started with gppm, follow these steps:

1. **Clone the repository**:
    ```sh
    git clone https://github.com/crashr/gppm.git
    cd gppm
    ```

2. **Set up a virtual environment**:
    ```sh
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Install dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

## Basic configuration
1. **Copy configuration example**:
    ```sh
    cp gppmd_config.yaml.example gppmd_config.yaml
    cd gppm
    ```
2. **Set log_file_to_monitor to a path that gppm can read from and llama.cpp can write to**:

## Usage

To run gppm, use the following command:

```sh
python3 gppmd.py
