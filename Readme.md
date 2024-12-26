# Devpool

Devpool is a quick and easy way to set up a Bitcoin Ordinals development environment macOS using the regtest environment. It leverages Docker to spin up the necessary services and provides a simple command line interface to manage the environment.

## Services

- Bitcoin Core: http://localhost:18443
- Ord: http://localhost:80
- Electrs: http://localhost:50001
- Mempool: http://localhost:8080

## Quick Start

1. Clone the repository:

```bash
git clone https://github.com/ordin8/devpool.git
cd devpool
```

2. Run the `start` command to start the services:

```bash
./devpool start
```

3. Once the services are running, you can use the `ord` command to interact with the Ord wallet:

```bash
./devpool ord wallet create
```

4. You can also use the `bitcoin-cli` command to interact with the Bitcoin Core node:

```bash
./devpool bitcoin-cli getblockchaininfo
```

5. To stop the services, use the `stop` command:

```bash
./devpool stop
```

6. To restart the services, use the `restart` command:

```bash
./devpool restart
```

## License

MIT
