# Hint Solver
Solvers presented in the IACR publication in EUROCRYPT 2025, see [https://ia.cr/2024/1211](https://ia.cr/2024/1211) for an extended version.

## Requirements:
- Rust
- Python >= 3.9, <=3.10
- maturin (tested with 1.5.1 and 1.8.2; some earlier versions give no warnings)
- venv
- tmux (if ``start_runs.sh`` or ``start_runs_all_threads.sh`` is being used)

## Setup environment:
- Install rust and maturin (see [https://www.rust-lang.org/tools/install](https://www.rust-lang.org/tools/install) and [https://www.maturin.rs/installation.html](https://www.maturin.rs/installation.html))
- Make sure a python version >= 3.9 is installed
- Use setup.sh to create a virtual environment (under ``.env/``), install required python packages, and compile the rust files
- Note that you need to source ``setup.sh``, i.e., ``source setup.sh``
- Note that the size of the message (``SZ_MSG``) needs to be adapted in the rust code, which needs to be recompiled after changing it.
