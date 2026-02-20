## LouLouLibs

Open-source tools for finance research and data workflows. Julia packages and Go CLI tools — mostly born out of academic finance work.

### Finance

| Package | Description |
|---|---|
| [**FinanceRoutines.jl**](https://github.com/LouLouLibs/FinanceRoutines.jl) | Import CRSP, Compustat, Fama-French factors, and GSW yield curves from WRDS or the web. Estimate betas with rolling windows. |
| [**wrds-download**](https://github.com/LouLouLibs/wrds-download) | Terminal app (TUI + CLI) to browse and download WRDS PostgreSQL data. Parquet & CSV output, Duo 2FA. Pure Go, cross-platform. *Vibe coded.* |

### Data

| Package | Description |
|---|---|
| [**BazerData.jl**](https://github.com/LouLouLibs/BazerData.jl) | `tabulate`, `xtile`, `winsorize`, `panel_fill`, `tlag`/`tlead` — Stata-flavored data manipulation for DataFrames.jl. |
| [**TigerFetch.jl**](https://github.com/LouLouLibs/TigerFetch.jl) | Download US Census TIGER/Line shapefiles. CLI and Julia interfaces for states, counties, water areas, and more. |

### Utilities

| Package | Description |
|---|---|
| [**NickelEval**](https://github.com/LouLouLibs/NickelEval) | Julia FFI bindings for the [Nickel](https://nickel-lang.org/) configuration language. Evaluate Nickel, convert types, export to JSON/TOML/YAML. *Vibe coded.* |
| [**BazerUtils.jl**](https://github.com/LouLouLibs/BazerUtils.jl) | Configurable logger with per-level file output, module filtering, and multiple formats (`pretty`, `log4j`, `syslog`). |

### Install Julia packages

All Julia packages are available through the [loulouJL](https://github.com/LouLouLibs/loulouJL) registry:

```julia
using Pkg
Pkg.Registry.add(url="https://github.com/LouLouLibs/loulouJL")
Pkg.add("FinanceRoutines")  # or any package above
```
