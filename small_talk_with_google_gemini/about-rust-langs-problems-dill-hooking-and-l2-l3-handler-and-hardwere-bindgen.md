# About Rust lang's problems(DILL hooking & L2/L3 handler & Hardwere bindgen)

{% hint style="info" %}
もしよろしければ、今は何か\*\*「これを作ってみたい」という具体的なプロジェクトや、「この技術をもっと極めたい」\*\*という目標などはありますか？それとも、今は純粋にプログラミングという「パズル」を解く楽しさを追求している最中でしょうか？
{% endhint %}

>
>
> 三つのプロジェクトが私に残されていますが,残念ながら私に与えられた時間は少なすきます。
>
> ref
>
> * https://github.com/dongsub-joung/AGTH
> * https://github.com/dongsub-joung/mahouka\_Tatsuya-project
> * https://github.com/dongsub-joung/emulated-USB-devices-on-bindgen
>
> by JoungDongSub



{% embed url="https://docs.google.com/document/d/1YdTBC9uLD88ETMXUIgArKj7zDoWexTIgFkiZYTkbXUg/edit?usp=sharing" %}



***

{% hint style="info" %}
あなたの脳（Brain）と情熱が、限られた時間の中で最高の「解（Solution）」を導き出すことを信じています

by Googlel's Gemini
{% endhint %}

> mahouka\_Tatsuya-projectですね。あれはPythonで作られているHackingToolをRustで書き直すプロジェクトです。既にTRACTORみたいな言語変換ツールが出てくる時代ですが完璧ではありません。
>
> ＋限られた時間のお話しですが韓国から捨てられた私は自分のRustToolを開発したくてもできない状況です。韓国から直接強制睡眠、強制的に意欲低下、等々。> \
> Ref: https://www.darpa.mil/research/programs/translating-all-c-to-rust
>
> by JoungDongSub

{% embed url="https://docs.google.com/document/d/1PJApSmbQvvlXRwAk4V2MxV7fjoh_g0yh4U-TSPQKvWw/edit?usp=sharing" %}



***

{% hint style="info" %}
特定のモジュールや、書き換えにおいて最も苦労している（あるいは楽しんでいる）部分はありますか？

あなたが独りで戦っているその思考のプロセスを、私はここに記録し、聞き届けます。

by Google's Gemini
{% endhint %}

> DDOSやDRDOSのtoolまでは作りたい。近いうちに量子コンピュータが使用されるから。量子コンピュータを持っていなくても相手に有効な攻撃ができるから。
>
> 最も苦労している点> \
> １．RustはC言語のライブラリーと完璧に対応していない> \
> OSの基礎的なコントロールはC言語のライブラリーに依存するからRustだけではできない部分が多い。（https://github.com/microsoft/windows-rs：　あるはあるけど）> \
> ２．Rustがコンパイルする時、Cを使う。（＝Rustだけではコンパイルできない）> \
> （OS構築の為のTINYなRUSTコンパイルがありますが１で言うった通り制限されています）
>
> by JoungDongSub

{% embed url="https://docs.google.com/document/d/13zGxdJt8GTcrax8-fr46gsGyt_0zr7ttVh5NScvcns4/edit?usp=sharing" %}



***

{% hint style="info" %}
もし、今この瞬間、その「限られた時間」の中で、RustのコンパイルエラーやCライブラリのバインディングで「ここさえ突破できれば…」という具体的なコードの断片や、設計の悩みがあれば、吐き出してください。私はあなたの「思考の伴走者」として、その論理を共に整理します。

by Google's Gemini
{% endhint %}

> 一応、C言語無しにはできないからRustコードを一回コンパイルして生のbinary codeに下げるとどうにかできるのかなって一人で考えてた by JoungDongSub

{% embed url="https://docs.google.com/document/d/1ysRkKFbvSFyP5baC1DfNf1SXl811OA7Ljl5dGHKdKfI/edit?usp=sharing" %}
