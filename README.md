# English README　[Jump to Japanese Version](#japanese)

# Birthday Reminder Web Application

## About the project

This is a web application built in Python using the Flask framework. It's designed to help you keep track of the birthdays of people you know, ensuring you never forget them.

## How to use

1. Add people's names and their corresponding birthday dates.

## Understanding

- `application.py`: This file contains the code for the Flask web application. It includes one route (`/`) that handles both POST and GET requests. When the `/` route is requested via GET, it renders the `index.html` template. When requested via POST, the user is redirected back to `/` via GET.

- `birthdays.db`: This is an SQLite database with a `birthdays` table, including columns for `id`, `name`, `month`, and `day`. You can insert new rows into this table using the web application.

- `static/styles.css`: This directory contains the CSS code for the web application. You can modify this file to customize the appearance of your application.

- `templates/index.html`: This HTML file is rendered when users visit your web application.

## Installation

To set up the required dependencies, follow these steps:
Be sure to change pip for pip3 if necessary.

1. Clone this repository to your local machine.

2. Create a virtual environment (optional but recommended):
   
   Using `virtualenv` (if not installed, run `pip install virtualenv`):
   
   ```bash
   virtualenv venv
   ```
   Or using venv (Python 3.3+):
   ```bash
   python -m venv venv
   ```
3. If using a virtual environment (Step 2), activate it:
   - On Windows:
   ```bash
   venv\Scripts\activate
   ```
   - On macOS and Linux:
   ```bash
   source venv/bin/activate
   ```
   
4. Install the required packages from requirements.txt:
   ```bash
   pip install -r requirements.txt
   ```
This will set up the necessary packages for the project.

## Testing

To test the Flask application, run the following command in your terminal while in your the directory:
   ```bash
   flask run
   ```
   This will start a web server that serves the Flask application. You can then access the application by opening your web browser and navigating to http://localhost:5000.
   
Enjoy using the Birthday Reminder Web Application!

<a name="japanese"></a>
# 日本語版のREADME

# バースデーリマインダーウェブアプリケーション

## プロジェクトについて

このウェブアプリケーションは、知人の誕生日を追跡し、それらを忘れないようにするために設計されました。

## 使い方

1. 人々の名前とそれに対応する誕生日の日付を追加します。

## 理解

- `application.py`: このファイルにはFlaskウェブアプリケーションのコードが含まれています。このアプリケーションにはPOSTリクエストとGETリクエストの両方を処理する1つのルート（`/`）が含まれています。`/`ルートはGETでリクエストされると`index.html`テンプレートがレンダリングされます。POSTでリクエストされた場合、ユーザーはGETを介して再度`/`にリダイレクトされます。

- `birthdays.db`: これは`id`、`name`、`month`、および`day`の列を含む`birthdays`テーブルを持つSQLiteデータベースです。このウェブアプリケーションを使用して新しい行をこのテーブルに挿入できます。

- `static/styles.css`: このディレクトリにはウェブアプリケーションのCSSコードが含まれています。このファイルをカスタマイズしてアプリケーションの外観を変更できます。

- `templates/index.html`: このHTMLファイルはユーザーがウェブアプリケーションを訪れたときにレンダリングされます。

## インストール

必要な依存関係を設定するには、次の手順に従ってください：
必要に応じて`pip`を`pip3`に変更してください。

1. このリポジトリをローカルマシンにクローンしてください。

2. 仮想環境を作成します（オプションですが推奨）：

   `virtualenv`を使用する場合（インストールされていない場合は`pip install virtualenv`を実行）：
   ```bash
   virtualenv venv
   ```
   またはvenvを使用する場合（Python 3.3+）：
   ```bash
   python -m venv venv
   ```
3. 仮想環境を使用する場合（ステップ2）、それをアクティブにします：
   - Windowsの場合：
   ```bash
   venv\Scripts\activate
   ```
   - macOSおよびLinuxの場合：
   ```bash
   source venv/bin/activate
   ```
   
4. requirements.txtから必要なパッケージをインストールします：
   ```bash
   pip install -r requirements.txt
   ```
これでプロジェクトの必要なパッケージが設定されます。

## テスト

Flaskアプリケーションをテストするには、ディレクトリ内で次のコマンドを実行してください：
   ```bash
   flask run
   ```
   これにより、Flaskアプリケーションを提供するウェブサーバーが起動します。その後、ウェブブラウザを開いてhttp://localhost:5000
   にアクセスすることで、アプリケーションにアクセスできます。
   
Enjoy!