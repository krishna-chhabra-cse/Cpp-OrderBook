# Cpp-OrderBook

A high-performance Limit Order Book (LOB) and Matching Engine implemented in modern C++. This project simulates the core functionality used by electronic exchanges, where buy and sell orders are matched using price-time priority.

## Features

- Supports Buy and Sell limit orders
- Price-Time Priority (FIFO) matching
- Order insertion, cancellation, and modification
- Automatic trade execution when prices cross
- Real-time order book updates
- Efficient data structures for low-latency processing
- Modular and extensible architecture

## How It Works

The engine maintains separate bid and ask books and continuously matches incoming orders against the best available prices. Orders are executed according to exchange-style rules:

1. Best price gets priority.
2. Orders at the same price are matched in FIFO order.
3. Partial fills are supported.
4. Remaining quantities are stored in the order book.

## Tech Stack

- **Language:** C++17/C++20
- **Data Structures:** STL containers, priority queues, maps
- **Build System:** CMake
- **Testing:** Unit tests (optional)

## Applications

- High-Frequency Trading (HFT) systems
- Quantitative Finance research
- Exchange and matching engine simulations
- Market microstructure analysis
- Learning low-latency systems design

## Future Improvements

- Market orders support
- Multi-threaded matching engine
- REST/WebSocket API
- Performance benchmarking
- Persistent trade logs
- Frontend visualization dashboard
- Historical replay and backtesting support

## Example Output
