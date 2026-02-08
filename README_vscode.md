# VSCode For Python
Python開発用 VSCode環境ファイル

## 便利なコマンド
- 仮想環境構築  
    ```bash
    python -m venv venv
    ```
- 依存関係インストール  
    ```bash
    pip install -r requirements.txt
    ```
- 型チェック（Pylance互換 / strict）  
    ```bash
    pyright
    ```
- flake8（E501 / W503 / W504 無視）  
    ```bash
    flake8 src --ignore=E501,W503,W504
    ```
- isort（設定ファイル使用）  
    ```bash
    isort src --settings-file .isort.cfg --check
    ```
- autopep8（E501 / W503 / W504 無視）  
    ```bash
    autopep8 -ir src --ignore=E501,W503,W504
    ```
- 循環的複雑度  
    ```bash
    radon cc -s src
    ```
- 実行コード数カウント  
    ```bash
    pygount --format=summary --suffix=py src
    ```
- インストール済みPythonライブラリのライセンス一覧  
    ```bash
    pip-licenses -f csv > pip-licenses.csv
    ```
- VS Code拡張機能一覧  
    ```bash
    code --list-extensions > extensions_list.txt
    ```
