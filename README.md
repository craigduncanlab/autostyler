# Autostyler

(c) 2019-2022 Craig Duncan www.craigduncan.com.au

This app will take plain text and transform into a .docx file in the output folder

It uses simple AI to infer styles by document type.

# Specifying input document type

Options (include one of theses lines at top of input file):

meta:legaldoc

meta:memo

meta:letter

# Notes

Double-forward-slash in the input file // can be used to indicate a comments (notes) line 

# Run from command line

(ensure you have python3 installed on your system)

```
python3 autostyler.py -n filename.txt
```

Options:

-n to specify 'notes on'

-o to specify an output folder.

# Workflow extensions

Use R Markdown and knitr to create your input text file from variables.

See example file : KnitExample.Rmd

Then run the following from an R Studio console:


```
rmarkdown::render(input = "~/Documents/Path/KnitExample.Rmd",intermediates_dir="~/Documents/Path/output",run_pandoc=FALSE)
```

This will produce a markdown output file with .md extension

Use this as the input file for the workflow above.