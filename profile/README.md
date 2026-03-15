## LouLouLibs

Open-source tools for finance research and data workflows. Julia packages and some CLI tools — mostly ideas from my academic work.

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
|----|----|
| [**xl-cli-tools**](https://github.com/LouLouLibs/xl-cli-tools) | View and edit Excel files from the terminal. `xlcat` renders xlsx/xls as markdown tables or CSV; `xlset` modifies cells preserving formatting. Rust, no runtime deps. *Vibe coded.* |
| [**go-xldiff**](https://github.com/LouLouLibs/go-xldiff) | Compare two Excel sheets and report added, removed, and modified rows. Text, JSON, and CSV output. Pure Go, cross-platform. |
| [**esync**](https://github.com/LouLouLibs/esync) | Watch local files and rsync them to a remote on every change, with a live TUI. Auto-imports `.gitignore`, daemon mode, SSH keepalive. Pure Go. *Vibe coded.* |
| [**bbtex**](https://github.com/LouLouLibs/bbtex)| Trying to parse LaTeX logs and use applescript to have a good LaTeX IDE in bbedit |



### Other Julia Packages 

| Package | Description |
|---|---|
| [**NickelEval**](https://github.com/LouLouLibs/NickelEval) | Julia FFI bindings for the [Nickel](https://nickel-lang.org/) configuration language. Evaluate Nickel, convert types, export to JSON/TOML/YAML. *Vibe coded.* |
| [**BazerUtils.jl**](https://github.com/LouLouLibs/BazerUtils.jl) | Configurable logger with per-level file output, module filtering, and multiple formats (`pretty`, `log4j`, `syslog`). |


### Claude Skills
I usually have claude write a skill for my use case after I have it code a utility. 
They are gathered at [`claude-skills`](https://github.com/LouLouLibs/claude-skills)


### Install Julia packages

All Julia packages are available through the [loulouJL](https://github.com/LouLouLibs/loulouJL) registry:

```julia
using Pkg
Pkg.Registry.add(url="https://github.com/LouLouLibs/loulouJL")
Pkg.add("FinanceRoutines")  # or any package above
```
