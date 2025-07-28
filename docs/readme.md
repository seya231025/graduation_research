# 1. バックエンドディレクトリに移動
cd backend

# 2. Python仮想環境の作成と有効化
python -m venv venv
source venv/bin/activate  # Windowsの場合は `venv\Scripts\activate`

# 3. 依存ライブラリのインストール
pip install -r requirements.txt

# 4. APIサーバーの起動
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000