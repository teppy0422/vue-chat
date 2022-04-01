> ### 事前準備
>> npmの更新  
>> Vue/CLIのインストール  

> ### 作成  
>> 起動:nmp run serve  
終了:control + C

> ### Vuetify  
>> vue add veutify

> ### Vue Router  
>>vue add router
>>>still proceed = y
>>>history mode? = y

> ### GitHub Pagesで公開
>> vue.confit.jsに下記を追加  
>> 標準ではoputputDirはdistだけどGitHub Pagesではdocsかrootが標準だから
>> publicPathはリポジトリ名にする
>>> outputDir: 'docs',  
>>> publicPath: '/vue-chat/'  

>> docsの作成  
>>> ターミナルで実行
>>>> npm run build  
>>> それらをコミットしてプッシュ

>> GitHubの設定
>>> 対象のリポジトリ > Setting > Pages > Source を/docsに変更してSave

>>> ここまでで閲覧可能になる

> ### トラブル  
>> サイトでリロードしたりURL直接アクセスで404エラーになる場合は下記ファイルを追加  
>>> $ touch public/_redirects  
>>>> /* /index.html 200  

