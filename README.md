

-----

# Bruteforce Password Cracker

A tool for cracking passwords using various attack methods.

## Features

  - **Bruteforce Attack:** Customizable character sets.
  - **Dictionary Attack:** Use pre-made wordlists.
  - **Smart Attack:** Based on user information.
  - **Hybrid Attack:** Combines dictionary attacks with mutations.
  - **Rainbow Table Attack:** Utilizes rainbow tables for cracking.
  - **High Performance:** Multi-threaded processing.
  - **GPU Acceleration:** For supported hash functions.
  - **GUI:** A graphical user interface for ease of use.

-----

## Command-Line Usage

```bash
python bruteforce.py --target <hash> --mode <mode> --length <max_length> [options]
```

### **Main Parameters:**

  - `--target` or `-t`: The target hash to crack.
  - `--mode` or `-m`: Mode (1=digits only, 2=letters only, 3=all characters).
  - `--length` or `-l`: Maximum password length.
  - `--dictionary` or `-d`: Path to the dictionary file.
  - `--hash-type` or `-ht`: Hash type (plaintext, md5, sha1, sha256, sha512, ntlm, base64).
  - `--threads` or `-th`: Number of threads.

### **Additional Parameters:**

  - `--rainbow-table` or `-rt`: Path to the rainbow table file.
  - `--smart-attack` or `-sa`: Enable smart attack.
  - `--hybrid-attack` or `-ha`: Enable hybrid attack.
  - `--targeted` or `-tg`: Enable targeted bruteforce.
  - `--optimize` or `-o`: Optimize character sets.

-----

## GUI Usage

```bash
python bruteforce_gui.py
```

The GUI provides a user-friendly interface for all program functions, with additional tabs for configuring advanced settings and user information.

-----

## Project Files

  - `bruteforce.py`: The main bruteforce module.
  - `bruteforce_gui.py`: The Graphical User Interface (GUI).
  - `hash_functions.py`: Implementation of hash functions and GPU acceleration.
  - `wordlist_generator.py`: The wordlist generator.
