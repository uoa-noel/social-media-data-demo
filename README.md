# Collecting and analysing social media data: A demo
This repository contains the notebook for a demo of using Twitter data I presented at [ResBaz Aotearoa 2022](https://resbaz.auckland.ac.nz).

[**View the demo**](smd-demo.ipynb)

## Set up on your own computer
If you want to run the demo notebook on your own computer, follow these steps.

You will need to be running Linux, or on Windows with [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).

1. Install `jq` and Jupyter Notebook. On Ubuntu (including inside WSL2), you can run `sudo apt install jq jupyter-notebook`. 
2. Clone this repository.
3. In a shell, run `pip install -r requirements.txt`. This will set up all the Python dependencies. Advanced users may wish to set up a Python virtual environment for this notebook first.
4. Run `python -m spacy download en_core_web_sm` - this will download and install the SpaCy language model needed in the notebook.
5. Register for a [Twitter Developer account](https://developer.twitter.com/), then run `twarc2 configure`. Twarc will prompt you for API credentials. Subsequent uses of twarc will be able to make requests to Twitter without asking for your credentials again.
6. You can now run Jupyter Notebook.`jupyter notebook`
A browser window should open showing the Jupyter Notebook interface. Click on `smd-demo.ipynb`.