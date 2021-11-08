# MarkdownConverter
Shell script to convert Markdown files to either pdf or html files. If the script is being executed in Mac OS X, then it opens the newly created file with *open* (shell built-in command); in Linux or other Unix systems the files are not automatically opened upon completion of the conversion.

The output file's name will be the same one as the input file's name but with either the .hmtl or .pdf file extension. 

**TLDR IMPORTANT NOTICE**: Right now this shell script does not add much value to the user, because its behaviour resembles just executing the pandoc command to convert a file to either html or pdf and then open the result. But the long-term goal would be to also incorporate different html and latex templates to the script to allow more design customization. In that case, using this script will definitely prove to be a relief for the user, since template configuration commands with pandoc tend to be quite long.

## Dependencies
**pandoc**, if pandoc is not present in the system, the script will issue an error and exit.
In order for pandoc to generate pdf files, it usually needs Latex generators (read the pandoc documentation for more details if a pdf file conversion does not work for you!).

## Usage
```
usage: MarkdownConverter --html | --pdf <input Markdown file name>
	--html : Convert input Markdown file to HTML
	--pdf : Convert input Markdown file to pdf
```
