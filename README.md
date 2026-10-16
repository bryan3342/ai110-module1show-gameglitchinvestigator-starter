# Game Glitch Investigator

## Description

A Streamlit number-guessing game supplied as an AI110 debugging exercise. The checked-in version is intentionally incomplete: `logic_utils.py` contains `NotImplementedError` stubs, and the app still has incorrect hints, inconsistent guess types, and incomplete reset behavior.

## Dependencies

- Python 3 and pip.
- `streamlit>=1.21.0`, `altair<5`, and `pytest`, as listed in `requirements.txt`.

## Technologies

Python, Streamlit, and pytest.

## Setup

```bash
git clone https://github.com/bryan3342/ai110-module1show-gameglitchinvestigator-starter.git
cd ai110-module1show-gameglitchinvestigator-starter
python -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

On Windows, activate the environment with `.venv\Scripts\activate` instead.

## Features

- Easy, Normal, and Hard difficulty controls.
- Guess submission, score display, attempt history, and a developer debug panel.
- Three tests for winning, high, and low guesses.
- A [reflection worksheet](reflection.md) for documenting bugs, fixes, and testing.

The exercise is to investigate the behavior, move logic into `logic_utils.py`, and make the tests pass. The tests expect `check_guess` to return a status string, while the current app function returns a tuple. These interfaces need to be reconciled during the exercise.

## Commands to run

```bash
python -m streamlit run app.py
python -m pytest
```

The test command is expected to fail against the unimplemented helper functions.

## Contributors

- Andrew Burke, credited in the starter's Git history.
- [Jamila Cocchiola (@jamjamgobambam)](https://github.com/jamjamgobambam), credited in the starter's Git history.

This copy is hosted by [@bryan3342](https://github.com/bryan3342). The inspected history contains no Bryan-authored implementation commits.
