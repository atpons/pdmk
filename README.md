# pdmk
Pandoc Markdown to any format with your template!

## Usage

1. Write pdmk metadata in your Markdown document

- `_pdmk_template`: pandoc template for your document (required)
- `_pdmk_output`: output extension (required)
- `_pdmk_arg`: you can use other arguments if you need

```markdown
---
_pdmk_template: template.tex
_pdmk_output: pdf
_pdmk_arg: --toc
...
---
```

2. Place template in your document directory or pdmk template directory
You can use pdmk template directory is `~/.pdmk/template`, while you can place template in your document directory.

3. Run
```shell
$ pdmk document.md
```

## Directory design
### Using pdmk template directory
```
~/.pdmk
└── template
    └── template.tex
```

### Using place template and document on same directory
```
mydocument
├── document.md
└── template.tex
```
