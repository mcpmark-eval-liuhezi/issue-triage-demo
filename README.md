# issue-triage-demo

A small demo project used in a graduate seminar on software maintenance. It exists so students can watch a real bug report travel the full path: file, triage, fix, review, and merge.

The project is a trivial report-export tool: it reads a local config file, renders a report, and writes the result to disk. It is intentionally buggy, and the issue tracker holds the work items for the in-class exercise.

## Installation

Install the demo project from source:

```bash
git clone https://github.com/mcpmark-eval-liuhezi/issue-triage-demo.git
cd issue-triage-demo
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

Then run the demo:

```bash
python -m issue_triage_demo --config config.yaml --output report.txt
```

## Usage

Point the tool at a config file and an output path. Missing or malformed configuration is a known rough edge (see the open issues).
