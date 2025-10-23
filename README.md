# Part 4 — Starter

Students should implement an extension of the current search. When searching with multiple words the user should be able to specify a search mode: either AND or OR. The merging of results can be reused from exercise 3. 
The focus is on extending the user interface (more specifically, the command line interface (CLI)) and extending the app's logic to provide logic for both search modes. 

## Run the app

```bash
python -m part4.app
```

## Check against the transcript

```bash
python -m part4.tests.check_transcript
```

## Where to work

- **ToDo 1:** Copy your solution from part 3 into `combine_results`, also copy the splitting of the raw string.
- **ToDo 2:** Introduce a new element to the command line interface (CLI): **A search mode**. 

  The search mode should enable the user to switch between two modes **AND** and **OR** (the **AND** mode is what we currently have in exercise 3). 
  To switch modes the user should be able to use the following command: ```:search-mode AND|OR```. The default mode should be `AND`.
  - **ToDo 2 — Part 1:** Follow the implementation of the highlight feature to implement the search mode feature in the user input while loop.
        
      After finishing this ToDo you will have a variable, e.g., `search_mode`, reflecting the currently chosen mode.
  - **ToDo 2 — Part 2:** Use that variable to control the logic in which `combine_results` is called.
