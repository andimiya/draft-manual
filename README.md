# 2017 Draft Manual

Edit and style in markdown/HTML, then generate a PDF.

## Editing
- Edit in Markdown, in the `index.md` file
- The gulp process will take your markdown and convert it into HTML and output into the `public/index.html` file.
If you make any changes in the `public/index.html` file, it'll get overwritten!
- Add your styles to `scss/styles.scss`, which will be compiled to `public/styles.css` through the gulp process

## Publishing notes
- Prince PDF's free version prints a small logo on the first page of any generated PDF, so I skip the first page and start the cover page on the second page.
- After the PDF is generated by Prince, we can remove the first page using a PDF editor.

## Run Locally
- `npm install`
- Run locally with `gulp`

## Generate a PDF
- Make sure you have Prince installed on your computer
- In your terminal, navigate to the folder you'd like to save the PDF to.
- Run this command `prince {URL} -o {name-of-pdf.pdf}`
example: `prince http://localhost:8282 -o testoutput9.pdf`

## Prince Installation Instructions
Do this if you've never used Prince PDF generator before:  
- $ tar xzf prince-9.0-macosx.tar.gz
- $ cd prince-9.0-macosx
- $ sudo ./install.sh

More instructions just in case:
https://www.princexml.com/doc/installing/
