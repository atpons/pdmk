# pdmk
Pandoc Markdownと好きなテンプレートでドキュメントを生成するためのツール

## Usage

1. pdmk メタデータをあなたのドキュメントのYAMLメタデータにに記入してください．

- `_pdmk_template`: 指定するテンプレートファイル名(必須)
- `_pdmk_output`: 出力ファイル拡張子
- `_pdmk_arg`: 他の引数を取る場合はここに記入してください

```markdown
---
_pdmk_template: template.tex
_pdmk_output: pdf
_pdmk_arg: --toc
...
---
```

2. テンプレートファイルを配置する
`~/.pdmk/template`にファイルを配置するか，ドキュメントと同じ位置にテンプレートファイルを配置してください．ドキュメントファイルと同じ位置に配置されたテンプレートファイルが優先して使用されます．

## ディレクトリ構成
### 共通場所にテンプレートファイルを配置するとき
```
~/.pdmk
└── template
    └── template.tex
```

### ドキュメントファイルと同じ位置にテンプレートファイルを配置するとき
```
mydocument
├── document.md
└── template.tex
```
