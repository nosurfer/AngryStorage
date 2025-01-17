# AngryStorage

This repository contains a solution for the [AngryStorage](https://web-kids20.forkbomb.ru/tasks/websrv2_angrystorage) task from the website [forkbomb.ru](https://forkbomb.ru/), which I solved by exploiting a race condition vulnerability. The original challenge involved understanding and leveraging concurrent execution to achieve the desired result.

I decided to rewrite the solution in C, focusing on implementing the exploit in a multithreaded environment using **pthreads** and the **libcurl** library for HTTP requests. This project serves as both a practical implementation of the exploit and a demonstration of handling concurrency in C.

## Getting Started

### Prerequisites

- **Python 3.x**: Ensure Python 3 is installed on your system. You can check by running:
```bash
python3 --version
```
- **C Compiler (gcc)**: Ensure you have a C compiler (like gcc) and the libcurl development library installed. You can install them on Linux with:
```bash
sudo apt-get install gcc libcurl4-openssl-dev
```
### Installation
```bash
git clone https://github.com/yourusername/AngryStorage.git
cd AngryStorage
```
## Running the Exploit Scripts
#### Python:
```bash
python3 ./exploit.py
```
#### C:
```bash
gcc ./exploit.c -o ExploitRaceCondition -lcurl && ./ExploitRaceCondition
```
