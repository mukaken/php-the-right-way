---
title: Vagrant
isChild: true
anchor:  vagrant
---

## Vagrant {#vagrant_title}

[Vagrant]を使えば、既知の仮想環境を使って自分用のボックスを作れて、その環境の構成も、たったひとつの設定ファイルだけでできる。
このボックスを手動で設定することもできるし、
[Puppet]とか[Chef]みたいな「プロビジョニング」ソフトにおまかせすることだってできる。
ベースとなる環境を配布できるようにしておけば、複数の開発環境をまったく同じ状態に構築できる。
複雑怪奇なコマンドを羅列した「環境構築手順書」だとかいうのもいらなくなるってこと。
ベース環境を「破棄」したり作りなおしたりするのもそんなに手間がかからないので、
まっさらな環境を用意するのもお手軽にできる。

Vagrantは、フォルダを作って、ホストと仮想マシンの間でコードを共有する。
つまり、ホストマシンで作ったり編集したりしたコードを、そのまま仮想マシンの中で実行できるっていうことだ。

### ちょっとした手助け

Vagrantを使い始めるときの手助けになるのが、これらのサービスだ。

- [Rove][Rove]: PHPなどのオプション込みで、一般的なVagrantビルドを作ってくれるサービス。プロビジョニングにはChefを使う。
- [Puphpet][Puphpet]: PHPの開発用の仮想マシンを作ってくれる、シンプルなGUI。
  **PHPに特化している。**
  ローカルVM以外に、クラウドサービスにデプロイすることもできる。
  プロビジョニングにはPuppetを使う。
- [Protobox][Protobox]: vagrant をラップしたウェブ GUI で、ウェブ開発向けの仮想マシンを用意してくれる。
  シンプルな YAML ドキュメントを使って、仮想マシン上にインストールするすべてものを制御できる。
- [Phansible][Phansible]: 使いやすいインターフェイスで、PHP プロジェクト用の Ansible Playbook を生成してくれる。


[Vagrant]: http://vagrantup.com/
[Puppet]: http://www.puppetlabs.com/
[Chef]: http://www.opscode.com/
[Rove]: http://rove.io/
[Puphpet]: https://puphpet.com/
[Protobox]: http://getprotobox.com/
[Phansible]: http://phansible.com/
