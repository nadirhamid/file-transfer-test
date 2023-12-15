# file-transfer-test

This Python module demonstrates a basic implementation of a secure file transfer system using Python sockets and AES encryption.

## Overview

The module consists of two main components: `server.py` and `client.py`. These components enable secure file transfer between a server and a client using a basic encryption mechanism (AES encryption from the `cryptography` library) over a network.

### Files

- `server.py`: Contains the server-side code that listens for incoming connections from clients and receives encrypted files sent by clients. It decrypts the received file and saves it as `received_file.txt`.

- `client.py`: Contains the client-side code that establishes a connection with the server, encrypts a file (`file_to_send.txt`), and sends it to the server for storage.

## Usage

1. Clone the repository:

    ```bash
    git clone https://github.com/nadirhamid/file-transfer-test.git
    ```

2. Install the required library:

    ```bash
    pip install cryptography
    ```

3. Run the server:

    ```bash
    python server.py
    ```

4. Run the client:

    ```bash
    python client.py
    ```

5. Verify the process:

    - After running the client, the server should display a message indicating the successful receipt of the file (`received_file.txt`).

## Note

- This is a basic implementation for educational purposes and doesn't cover all security aspects or error handling for a production environment.

- Consider enhancing the codebase w
