# LibdocでJsonファイルを作成できない

## 環境の記録
使用CODESYS バージョン 3.5.15.20
システム変数に下記を登録
- LIBDOC_CODESYS
  - "C:\Program Files (x86)\CODESYS 3.5.15.20\CODESYS\Common\CODESYS.exe"--Profile = "CODESYS V3.5 SP15 Patch 2"

- PATH
  - C:\Program Files (x86)\CODESYS 3.5.15.20\CODESYS\DocScripting\3.5.15.10

## 本文

下記のように UIが立ち上がってしまいこの状態から先に進まなくなってしまう。
中のコマンドを見ると --noUI とあるので正常な状況にではUIが立ち上がらずにjsonファイルを出力するのが正しい動作であると考えられます。
3.5.15.20でのバグなのか.... はたまた特有の設定があるのだろうか....

<!-- wp:image {"id":50,"sizeSlug":"large"} -->
<figure class="wp-block-image size-large"><img src="https://codesys.seiza-lol.com/wp-content/uploads/2020/11/image-1024x240.png" alt="" class="wp-image-50"/></figure>
<!-- /wp:image -->
