# jinja2とは

テンプレートエンジン

https://www.python.ambitious-engineer.com/archives/760

>jinja2とはpythonのweb開発でよく使用されるテンプレートエンジンライブラリの１つです。
>変わったネーミングですが、テンプレート→テンプル→神社となったそうです（神社とお寺とはち
>ょっと違いますが）。pipコマンドでインストールできます。

Flaskを入れたら勝手に入っていた

ここにある

https://www.python.ambitious-engineer.com/archives/1630

    mkdir templates
    vi index.html
でhtmlを作っておいて、{{}}的なもので埋め込み

かつ、.pyのほうで、`from flask import render_template`してから
`return render_template('index.html', values=values)`的なことをすれば良い
