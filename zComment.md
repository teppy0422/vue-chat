> ### 事前準備
>
> > npm の更新  
> > Vue/CLI のインストール

> ### 作成
>
> > 起動:nmp run serve  
> > 終了:control + C

> ### Vuetify
>
> > vue add veutify

> ### Vue Router
>
> > vue add router
> >
> > > still proceed = y
> > > history mode? = y

> ### GitHub Pages で公開
>
> > vue.confit.js に下記を追加  
> > 標準では oputputDir は dist だけど GitHub Pages では docs か root が標準だから  
> > publicPath はリポジトリ名にする
> >
> > > outputDir: 'docs',  
> > > publicPath: '/vue-chat/'

> > docs の作成
> >
> > > ターミナルで実行
> > >
> > > > npm run build  
> > > > それらをコミットしてプッシュ

> > GitHub の設定
> >
> > > 対象のリポジトリ > Setting > Pages > Source を/docs に変更して Save

> > > ここまでで閲覧可能になる

> ### トラブル
>
> > サイトでリロードしたり URL 直接アクセスで 404 エラーになる場合は下記ファイルを追加
> >
> > > $ touch public/\_redirects
> > >
> > > > /\* /index.html 200
