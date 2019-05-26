# Ubuntu用 Ansible セットアップサンプル

AnsibleでUbuntuの自動セットアップ。  
環境に応じてインストールするパッケージやバージョンは変更。  
サンプルは管理ユーザをadmuser、開発用ユーザをdevuserとしている。  
監視サーバにprometheusを使用している環境。


メインの実行ファイルを作成して、各ymlファイルをインクルードする形で進めるとよい。  

  - 構成
  ├sftp.yml # sftp用ユーザ作成、設定  
  ├awscli.yml # awscliインストール  
  ├default.yml  # OS初期設定、サーバ共通設定  
  ├grok-exporter.yml  # grok-exporterインストール・設定  
  ├mariadbclient.yml  # mariaclientインストール  
  ├mecab.yml # mecabインストール  
  ├nginx.yml # nginxインストール・設定  
  ├node-exporter.yml # node-exporterインストール・設定  
  ├php7.yml # php7インストール  
  ├process-exporter.yml # process-exporter設定  
  ├pyenv.yml # pyenvインストール  
  ├pyenv-devuser.yml # devuser用python実行環境設定  
  ├pyenv-install-python.yml # python関連インストール  
  ├R.yml # Rインストール  
  └RStudio.yml # RStudioインストール  
