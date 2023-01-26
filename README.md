# RapidCopy for GNU/Linux

![RapidCopy for Linux](https://github.com/KengoSawa2/RapidCopy/blob/master/SS/RapidCopy_Linux.png "RapidCopy for Linux")

#### 概要(About)

Windows系最速(?) のファイルコピー＆削除ツールFastCopy v2.11のGNU/Linux移植 独自発展版です。  
RapidCopy is portable version of FastCopy(v2.11) that runs GNU/Linux.  

Linux版はFastCopy v2.11のMac移植版である[RapidCopyPro for Mac]をベースとして作成されています。  
Linux ver was ported from RapidCopyPro for Mac  

#### ライセンス(License)
全ソースを二条項BSDライセンスで公開しています。  
Source Code license is [BSD 2-Clause License]  

#### 仕様／使用方法(Specification/Usage)

Japanese:
https://app.lespace.co.jp/file_bl/rapidcopy/manual/linux/index.html

English:
https://app.lespace.co.jp/file_bl/rapidcopy/manual/linux/index_en.html

基本的な仕様は[Mac ver]と共通です。  
Basically, usage and specification is same as the Mac version.  

#### インストール(install)
CentOS7.2以降およびUbuntu16.04,18.04向けには以下のバイナリがあります。
(ライブラリはすべて同梱されているので、単体で動作します)

The following binaries are available for CentOS 7.2(or later) and Ubuntu 16.04 and 18.04.
(All libraries are included,so Work with standalone)

https://github.com/KengoSawa2/RapidCopy/tree/master/static_bin

#### ビルドについて(to Build)
以下のディストリビューションでコンパイル、起動確認をしています。  
We checked next Linux distribution.  

OS:CentOS7.2(x64)  
必須ライブラリ(Required Library):libacl,libbsd,libattr  

OS:Ubuntu16.04 LTS(x64) and Ubuntu18.04 LTS(x64)  
必須ライブラリ(Required Library):libattr1-dev,libbsd-dev,libacl1-dev,libgl1-mesa-dev  

いずれの環境でもコンパイルにはQt5.6以降とQtCreatorが必要です。 
環境によってはg++などのインストールが必要かもしれません。  
QtCreatorを起動して、rapidcopy_main.proを読み込んでください。
Qtのダウンロードは以下のURLから行えます。

Qt Library(5.6 or later) and QtCreator are necessary to make.
You might need to be installed other library, such as g++,depending on your environment.  
Start up QtCreator and read project file "rapidcopy_main.pro"
Qt Framework can download here.

https://www.qt.io/

デフォルトではubuntuをターゲットとしています。  
CentOS7でコンパイルする場合はrapidcopy_main.proのLIBS行を変更してください。  
Default target is Ubuntu.
If you want to compile in CentOS7. Change the "LIBS" line of rapidcopy_main.pro.

#### TODO
- 未使用変数及びインタフェースのリファクタリング,コンパイラ警告潰し,未使用コード整理(code refactoring)
- ご本家FastCopy3.xxの各種新機能の取り込み(The great original FastCopyv3.xx function import)
- GNOME,KDEなどの各種デスクトップ環境へのインストール対応(support GNOME,KDE install/uninstall)
- Ubuntu Software Center対応(support Ubuntu Software Center)
- etc....

   [help]: <https://github.com/KengoSawa2/RapidCopy/tree/master/help>
   [RapidCopy]: <https://itunes.apple.com/jp/app/rapidcopy/id975974524>
   [Mac ver]: <http://www.lespace.co.jp/file_bl/rapidcopy/manual/index.html>
