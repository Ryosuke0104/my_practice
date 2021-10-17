# my_practice
自分の練習を保存する

適当に書いたコードや公開されていて、これからの学習で有用そうなものを置いていく


gradについて
Pytorch では、逆伝搬で勾配を計算した際に、以前に計算した勾配がある場合はそれに加算する形になっています。
今回の勾配 = 前回計算した勾配 + 今回計算した勾配
この仕様は RNN などのモデルでは有用なのですが、そうでない場合は前回計算した勾配を0で初期化する必要があるので、その場合は backward() を呼び出す前に zero_grad() を行う必要があります。
