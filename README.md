### 1. Introduction
This README provides step-by-step instructions to convert a Python Jupyter notebook into a Quarto document. It also covers how to edit the Quarto document, including adding images and references.

### 2. Prerequisites

Ensure you have the following installed:

- **Python**: Version 3.x
- **Jupyter Notebook**: You can install it via pip if not already installed (`pip install notebook`).
- **Quarto**: Download and install Quarto from [quarto.org](https://quarto.org/docs/get-started/).

### 3. Step-by-Step Guide

#### 3.1 Convert Jupyter Notebook to Quarto

1. **Create a Jupyter Notebook**:
   - Create your Python Jupyter notebook as usual, including your code, markdown cells, and outputs.
   - Save the notebook (`.ipynb` file).

2. **Convert the Notebook to Quarto**:
   - Open your terminal or command prompt.
   - Use the following command to convert the notebook to a Quarto document:
     ```bash
     quarto convert jupyter_notebook.ipynb -o output_file.qmd
     ```
   - This will generate a Quarto markdown file (`.qmd`).

#### 3.2 Editing in Quarto

1. **Add Images**:
   - You can add images to your Quarto document using markdown syntax:
     ```markdown
     ![Image Description](path/to/image.png)
     ```
   - To add images from a URL:
     ```markdown
     ![Image Description](https://example.com/image.png)
     ```

2. **Add References**:
   - You can manage references by creating a `bibliography.bib` file with your references in BibTeX format.
   - Link the bibliography file in your Quarto document header:
     ```yaml
     ---
     title: "Your Document Title"
     author: "Your Name"
     bibliography: bibliography.bib
     ---
     ```
   - Cite references in your text using the following syntax:
     ```markdown
     This is a citation [@citation_key].
     ```

3. **Other Edits**:
   - You can add headers, footnotes, and other markdown features as needed.
   - Customize the layout by editing the YAML header.

#### 3.3 Render the Quarto Document

1. **Render to HTML or PDF**:
   - Use the following command to render your Quarto document to HTML or PDF:
     ```bash
     quarto render your_document.qmd
     ```
   - This will generate the output in the specified format.

### 4. Example Workflow

Here is an example workflow:

1. Create a Jupyter notebook with your Python analysis.
2. Convert the notebook to Quarto (`your_notebook.qmd`).
3. Edit the Quarto document to add images, references, and customize formatting.
4. Render the document to your desired format (HTML, PDF).

### 5. Conclusion

This guide provides the basics for converting a Jupyter notebook to Quarto and customizing the document. For advanced features, refer to the [Quarto documentation](https://quarto.org/docs/guide/). This is the [DSCI book by UBC](https://ubc-dsci.github.io/reproducible-and-trustworthy-workflows-for-data-science/materials/lectures/08-reproducible-reports.html#).