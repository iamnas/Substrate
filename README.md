# Substrate Project

This project includes two components:  
1. **Substrate Node Template** - A custom Substrate blockchain node.  
2. **Substrate Front-End Template** - A front-end interface for interacting with the Substrate blockchain.

---

## Project Structure

```
/
├── substrate-node-template      # Custom Substrate node implementation
└── substrate-front-end-template # Front-end interface for the Substrate node
```

---

## Prerequisites

Ensure you have the following tools installed:

- **Rust** (for building the node): [Install Rust](https://www.rust-lang.org/tools/install)
- **Yarn** (for managing front-end dependencies): [Install Yarn](https://yarnpkg.com/getting-started/install)

---

## Running the Substrate Node

To set up and run the **Substrate Node**:

1. Navigate to the `substrate-node-template` directory:
   ```bash
   cd substrate-node-template
   ```

2. Build the node in release mode:
   ```bash
   cargo build --release
   ```

3. Start the node in development mode:
   ```bash
   ./target/release/node-template --dev
   ```

   > The `--dev` flag runs the node with a temporary state, ideal for testing.

4. The node should now be running locally on `127.0.0.1:9944`.

---

## Running the Substrate Front-End

To set up and run the **Front-End Template**:

1. Navigate to the `substrate-front-end-template` directory:
   ```bash
   cd substrate-front-end-template
   ```

2. Install the dependencies:
   ```bash
   yarn install
   ```

3. Start the development server:
   ```bash
   yarn run dev
   ```

4. Open your browser and navigate to:
   ```
   http://localhost:8000
   ```

5. The front-end interface should now connect to your local Substrate node.

---

## Notes

- Ensure the Substrate node is running **before** starting the front-end to allow proper connectivity.  
- The default WebSocket RPC endpoint for the node is `ws://127.0.0.1:9944`.  
- Use the front-end interface to interact with the node, view account balances, and perform transactions.

---

## Resources

- [Substrate Documentation](https://docs.substrate.io/)  
- [Substrate GitHub Repository](https://github.com/paritytech/substrate)  

---

Enjoy building with Substrate! 🚀