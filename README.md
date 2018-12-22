# stream
プログラムにおけるストリームについて

## ストリームの概念
ストリームは、名前の通りデータが流れてくるという概念です。配列と同じように複数のデータを扱う時に使いますが、配列より一般的な概念です。



配列には次のような制限があります。
1. 保存できる領域が有限
2. まだ存在していないものを扱えない

1はコンピューターの制約です。コンピューターのメモリは有限です。何億ものデータが入った配列を扱うことは不可能ではないですが、現実的ではありません。多くの場合そんな大きな場所はコンピューターの中にはないのです。

2について、例えばユーザーの購買行動ログを扱う場合を考えてみましょう。過去のデータは量が多くなければ配列で扱えるかもしれません。ですが、未来の場合はどうでしょう。これは配列で扱うことはできるでしょうか。答えはNoです。配列は実際に存在してるものしか扱えません。



ストリームにはこのような制限はありません。ストリームは無限のもの、まだ存在しないものを扱えるのです。
こう聞くと、とても難しいように感じるかもしれませんが、私たちはこの概念をいつでも使っています。


例えば、水について考えてみましょう。

私たちは毎日水を飲みますが、どうして家に一生分の水を置かないのでしょうか？場所がないからです。蛇口を捻れば水が出てきますが、これは文字通りストリームなのです。一生分で使う水の量というと想像もつきませんが、私たちはストリームという概念を用いることでこの大きな量を扱うことができるのです。


殆どの場合は蛇口を捻れば水が出ますが、断水しているかもしれません。言い換えると、私たちから見ると水が存在しているかどうかは分かりません。蛇口を捻って水が出るという事象は、「水が存在するかどうかは不確定だったが、蛇口を捻ったら水の存在が確定した」と捉えることもできます。これは蛇口を捻る時点では不確定だった要素を扱っていると言えます。


このような例は、そこら中にあります。物流の殆どはストリームとして捉えることができます。私たちが生きている世界も、ある時点での世界のスナップショットが時系列に流れていくストリームと捉えることができます。ストリームという概念は一般的すぎる故に理解が難しいです。


## プログラミングの世界でのストリーム
