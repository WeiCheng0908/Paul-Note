# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## MkDocs Documentation 設置基本法則
直接到documentation了解設置過程  
1. 新增功能時，大部分都要先在"mkdocs.yml"做設定  
2. 某些功能需要install package，某些要新增資料夾，端看documentation的描述  

## Material Theme Feature
[setting documentation](https://squidfunk.github.io/mkdocs-material/setup/)

### [Material 新增留言板](https://squidfunk.github.io/mkdocs-material/setup/adding-a-comment-system/)
需要override mkdocs自動產生的網頁原始碼，因此會有比較特別的設定
