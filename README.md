# ブランチ作成

### <a name="anchor1-2">リリースブランチの作成</a>

リリースが決定した場合、決定時点のコードでリリースブランチを作成する。

1. ローカルPCにて任意の場所で右クリックし、「TortoiseSVN」⇒「Repo-browser」を押下
1. URLに下記を指定して「OK」を押下
    - `https://r.svn.ne.jp/cmic/svn/NewSMOMO/branches/Release`
1. 「Repository Browser」ウィンドウの右枠を右クリックして「Create folder」を押下
    1. 「New name」にて「yyyymmdd(リリース日)_[SMOMO|SMONEY|SMART|API]」を指定して「OK」を押下  
        - すでに作成済みの場合、末尾に「.n」で1始まりの連番を振る
        - 複数同時にリリースする場合、"-"で繋ぐ
    1. 「Entry Log Message」にて下記を指定して「OK」を押下
        - yyyy-mm-dd リリースブランチ作成
1. 「Repository Browser」ウィンドウの上部URLに下記を指定して移動
    - `https://r.svn.ne.jp/cmic/svn/NewSMOMO/trunk`
1. 右枠よりリリース対象となるフォルダを右クリックし、「Copy to」を押下
    - Webアプリケーション ⇒ 「SMFApp」フォルダ
1. 「Copy to」ウィンドウのURLに下記を指定
    - `https://r.svn.ne.jp/cmic/svn/NewSMOMO/branches/Release/{リリースフォルダ}`
1. 「OK」ボタンを押下してブランチを作成
