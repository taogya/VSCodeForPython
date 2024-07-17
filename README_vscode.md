# VSCode For Python
Python開発用 VSCode環境ファイル

## 便利なコマンド
- 仮想環境構築 <br>
    ```
    $ python -m venv venv
    ```
- インストール済みPythonライブラリのライセンス一覧 <br>
    ```
    $ pip-licenses -f csv > pip-licenses.csv
    ```
- vscode 拡張機能一覧表示 <br>
    ```
    $ code --list-extensions > extensions_list.txt
    ```
- 実行コード数カウント <br>
    ```
    $ pygount --format=summary --suffix=py app
    ```
- 循環的複雑度 <br>
    ```
    $ radon cc -s app
    ```