
## hisecurity.org的source文件

网页使用[Hugo](https://gohugo.io/)生成，使用的theme为[hugo-book](https://github.com/hotosm/hugo-book)，让开发者只需专注内容

本网站在配置文件config.toml中enable了menu功能，网页左边的menu顺序参考/menu/index.md。如果没有enable menu功能，左边索引的顺序由content/docs/中的目录生成

同时网页使用了Github的Actions功能，在.github/workflows/pages.yml中配置，由于部署了DEPLOY_KEYS，可以自动将pg_source branch中的网页build，生成于public文件夹，deploy到master branch。每次push后Github自动执行流程，不需要额外操作，developer可以在Actions tab中观察进度。
