# dir-sync
High-performance, type-safe directory synchronization tool utilizing Python MP/MT, Pydantic validation, and structured logging.

## Key Features

* **Hybrid Concurrency Architecture:**
    * Uses `multiprocessing` for CPU-intensive diff calculation.
    * Uses `multithreading` for I/O-bound directory scanning, file transfer and deletion operations.
* **Type Safety & Validation:** Configuration management is handled via **Pydantic**, ensuring strict schema validation and runtime type checking.
* **Enterprise-Grade Observability:** Replaces standard outputs with structured **Logging** for detailed auditing and easier debugging.
* **Full CRUD Synchronization:** Handles Copy, Update, Directory Creation, and Deletion.
* **Dry-run:** Using a special flag, it is possible to simulate synchronisation operations instead of actually performing them.

## Tech Stack

* **Language:** Python 3.11+
* **Validation:** Pydantic
* **Concurrency:** `multiprocessing`, `threading`, `concurrent.futures`
* **Logging:** Native Python `logging` module
* **Testing** unittest framework

## Installation & Usage

1.  Open the Notebook in Google Colab:
    [![Open In Colab](https://colab.research.google.com/drive/10105fx0sr0jFXR4WpjIiC1KroBDgbEtW#scrollTo=acb1e485)

2.  Configure source and destination paths in the configuration cell and run.

## Disclaimer

This tool performs destructive actions (file deletion) to ensure source-destination mirroring. Use with caution.

## License

Distributed under the MIT License. See `LICENSE` for more information.
