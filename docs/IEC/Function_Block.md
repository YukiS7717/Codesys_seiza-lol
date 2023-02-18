# Function Block

## 概要
Codesysのプログラミングにおいて基本となる概念になります。
他のプログラミング言語における関数のような位置づけの機能です。
基本的に3S社やその他メーカー製のFunction Block(以下FB)やFunctionを組み合わせてプログラミングを行います。
自作のFBやFunctionを作成して使いまわしたり、ライブラリ化することで工数を減らすことが容易であることがCodesysの利点でもあります。

## Function Block (FB)
FBは内部で変数を保持して、返り値を持たない関数です。
FB単体で機能を持たせたり、モーションコントロールでいえばサーボON、OFFやJOG動作を行う際に使用します。
Execute型とEnable型の2つの型があります。
動作の流れは2つの型で共通で下記の動作手順を踏みます。
Execute(Enable) → Busy → Done(Status) ：()はEnable型

## Execute型
Execute型はExecute変数(起動変数)がTRUEになると起動し、DoneがTRUEになるとFB内部の動作が停止します。

## Enable型
Enable型はEnable変数(起動変数)がTRUEになると起動し、StatusがTRUEの間、目的の機能や設定を有効にします。

> CODESYSで新規にLibraryを作成する際に CODESYS Library を選択するとフォルダ構成が作成されていますので活用してみてください。
>FBの状態遷移が正しくなるような基本的な構成を作成しておくとPLC Open規格のFBを作成することが容易になりますのでお勧めします。
