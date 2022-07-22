Viano/Vishal: Issue #1072 Allow code snippets drag and drop into existing notebook cells · Issue #1072 · elyra-ai/elyra (github.com)

When searching for an issue on Elyra we were told to look for an issue labeled as “good first issue” so we decided to do Issue 1072. 
Issue 1072 is to add a drag and drop feature for code snippets directly into a notebook cell (similar to insert function). 
After looking through the codebase and working on it for around two weeks we realized the issue was more complicated than it first seemed so we went to Karla who specializes in the Elyra front end for help.
We discussed that currently the drag and drop feature is coded to create a new cell above the cell you are currently hovered over. In order to implement this feature, we would have to have the code differentiate between a hover over an existing cell to replace that cell, and a hover between cells to add a new cell. 
The issue was there was no listener between cells. We talked with Karla and showed her the part of the code we were looking at. She discovered that by dragging text into cells they would replace the cell, meaning there was code in place for drag and drop cell replacement. 
Eventually though she came to the same conclusion we did. She said that one drag and drop feature could be picked but implementing both drag and drop features would not be simple. 
To accomplish this is not possible in Elyra; it would need to be updated in the JupyterLab source code. 
She summed up our conversation in the comment below and removed the “good first issue” label.

<img src="ImageKarla.png" />




