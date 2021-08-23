# Accordion widget for displaying solutions in Jupyter notebook

Accordion widget for quick reveal/hide solution in Jupyter notebooks. Can be Python code, Markdown, or a mix of both.

The function `show()` in the module `show_solutions.py` reads the file `week01_solutions.txt` which contains solutions to all exercises, and retrieves the solution tagged for a particular exercise to display it in an accordion widget. Run the top cell in the notebook to import the function, then use the command `show('exercise_tag')` to display the appropriate solution widget.


### Required

- [ipywidgets](https://ipywidgets.readthedocs.io/en/latest/)
- [nbconvert](https://nbconvert.readthedocs.io/en/latest/)


### Export to HTML

- Display all accordion widgets in the notebook by running the `show(..)` commands.
- Save the widget state: in Jupyter Notebook, in the menu bar, select Widgets > Save Notebook Widget State.
- Save and terminate the notebook (File > Close and Halt).
- Run `nbconvert` to export the HTML file: `jupyter-nbconvert MWE.ipynb --to HTML --output MWE.html`
