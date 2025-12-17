# Resume build with Hugo, printed to PDF with weasyprint

## save as PDF: 
`
weasyprint .public/cv/index.html cv.pdf
`

## structure: 
- /data
    - .toml files with the data that actually populates the resume
- /content
    - contains cv.md, which specifies the orders the sections are displayed
- /layouts
    - /_default
        - cv.html
            - MASTER FORMAT FILE: header section defined in here, then specifies how content displays
        - /_markup
            - apply formatting to markup sections written in /content
    - /shortcodes
        - THE .html FILES IN HERE DEFINE THE LAYOUT OF EACH SECTION
- /assets
    - CSS goes here
