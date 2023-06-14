# AES Encryption and Decryption

This repository contains a simple implementation of AES encryption and decryption using the Go programming language. It demonstrates how to securely encrypt and decrypt data using the AES block cipher algorithm with Galois/Counter Mode (GCM) for authenticated encryption.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Usage](#usage)


## Introduction

The `main.go` file in this repository contains functions for encrypting and decrypting data using the Advanced Encryption Standard (AES) algorithm. AES is a widely-used symmetric encryption algorithm that operates on fixed-size blocks of data. The implementation in this code uses AES with a 256-bit key and Galois/Counter Mode (GCM) for authenticated encryption.

The `encrypt` function takes a plaintext byte array and a key byte array as inputs and returns the ciphertext. It generates a random nonce, encrypts the plaintext using AES-GCM, and appends the nonce to the ciphertext.

The `decrypt` function takes a ciphertext byte array and a key byte array as inputs and returns the decrypted plaintext. It extracts the nonce from the ciphertext, then uses AES-GCM to decrypt the remaining ciphertext and verify its authenticity.

## Prerequisites

To run the code in this repository, you need to have Go installed on your system. You can download and install Go from the official Go website: https://golang.org/

## Usage

1. Clone this repository to your local machine using the following command:

2. Navigate to the repository's directory:

`cd project-directory`

3. Open the `main.go` file and replace the placeholder `"YOUR KEY HERE"` with your desired encryption key.

4. Build and run the code using the following command:

`go run main.go`

The output will display the original plaintext and the decrypted plaintext to verify the correctness of the encryption and decryption processes.




