# Demo script

## Parameterized Notebook demo
### Papermill
> Talking point: To automate Notebooks a **command line interface** to execute them would be handy. Papermill is an open source tool you could use to run Notebooks from a command line interface. **Papermill lets you execute Notebooks and parameterize Notebooks**.
1. Login using "az login" before the demo and have things ready. This way there will be no login prompts during the demo.
2. Show KqlmagicParameterizedQuery.ipynb in ADS, and what the Notebook does
3. Jump to powershell command prompt:
  1. Execute Notebook for Florida using Papermill
    - papermill .\KqlmagicParameterizedQuery.ipynb .\StormEventsFlorida.ipynb -p stateFilter "FLORIDA"
  2. Execute Notebook for Washington using Papermill
    - papermill .\KqlmagicParameterizedQuery.ipynb .\StormEventsWashington.ipynb -p stateFilter "WASHINGTON"
  3. Open both Notebooks in ADS and show the results
  4. Use split view to have some fun

> Talking point: This opens up new opportunities for how notebooks can be used. For example: 1) If you have a multi-region service, you might want to run the same **analysis on different regions using parameterization**. If you find any issues, you might want to open incidents on it or mitigate the issue. 2) If you find a particular issue, you might want to run another Notebook to diagnose further. You can now **programmatically build  workflows**.

> Once you capture these important steps into Notebooks, you can execute them yourself manually, automate them and run them in the environment of your choice. **Create once and use everywhere**.

### Run with parameters
> Azure Data Studio provides an easy way to **input parameters manually** and re-run the Notebook.
1. Click on "Run with parameters" button on the top right.
2. Type in "ILLINOIS"; into the input box and execute.

> Azure Data Studio creates a **copy of the file** for you so that you do not overwrite the original, and then it is available for you to store as a separate copy.