# Autostyler

(c) 2019-2022 Craig Duncan www.craigduncan.com.au

This app will take plain text and transform into a .docx file in the output folder

It uses simple AI to infer styles by document type.  In other words, I'm using a kind of 'no markup', but that's not completely true, because even ordinary writing is a kind of markup, if you know how to interpret it.  There's meaning in everything!

It will turn this:

![InputPage](images/input.png?raw=true)

into this:

![OutputPage](images/output.png?raw=true)

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