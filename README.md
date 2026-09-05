
 # Part1DataPipelines

 ## Overview

 This project contains PySpark-based data-pipeline work for the HDB Part1 submission. The primary artifact is the notebook `Part1DataPipelines.ipynb` which documents pipeline logic and example outputs. The pipelines are written for PySpark and can be executed interactively in Visual Studio Code using your `Python 3.11.7` kernel.

 ## Key reviewer notes
 - PySpark is required. Jupyter is optional — you do not need a virtual environment if you use the system/kernel Python `3.11.7` that already has the required packages installed.
 - Ensure Java (8/11+) is installed and available on `PATH`.
 - PySpark version used/tested: `3.5.6`

 ## Prerequisites
 - Java 8/11 or newer
 - Python 3.8+ (this project targets Python 3.11.7 in reviewers' environment)
 - PySpark (or a standalone Spark distribution)
 - Packages: `pyspark`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn` (install into the kernel you will use)

 ## Install packages into the Python 3.11.7 kernel
 If you're using the `Python 3.11.7` kernel in VS Code (preferred in your case), install the Python packages into that interpreter. In a terminal where that `python` is active (or point to it explicitly):

 ```bash
 python -m pip install --upgrade pip
 python -m pip install pyspark pandas numpy matplotlib seaborn scikit-learn
 ```

 To confirm which `python` will be used by Spark when running `spark-submit`, set `PYSPARK_PYTHON` to that interpreter path (see below).


 ## Running and inspecting in Visual Studio Code
 1. Open the repository folder in VS Code.
 2. Install the **Python** extension (Microsoft). Optionally install **Jupyter** to view notebooks inline.
 3. Select the `Python 3.11.7` interpreter/kernel: click the interpreter selector (bottom-right) or use the Command Palette → `Python: Select Interpreter` and choose `Python 3.11.7`.
 4. To run the notebook interactively: open `Part1DataPipelines.ipynb` and use the Run All / Run Cell buttons. Outputs render inline in VS Code.


 ## Data and configuration
 - Raw source files are in the /RAW/ folder. 1 of the files are zipped as its too large to be uploaded to github
 - Cleaned file is in the output/Cleaned/Cleaned.csv.zip
