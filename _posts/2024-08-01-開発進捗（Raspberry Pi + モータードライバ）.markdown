こんにちは！西池袋ガチ研究所です。

今日は、先週組み立てた本番を想定したチキンを鳴らすための機構を鳴らすための作業をしました。

ひとまずRaspberry PiのGPIO経由でサーボモーターを動かしてみて、それができたらサーボドライバー経由で動かすのに挑戦しました。

サーボモーターをどのように動かせばよいかはまだ全く未着手なので、そこを詰めていきます。

Raspberry PiのGPIOピンについては、こちらの記事を参考にさせて頂きました。

https://qiita.com/Erytheia/items/f362a3d68e57cd088713

高いサーボモーターを破壊しないよう、安いサーボモーターで実験して動くのを確認
<iframe src="https://drive.google.com/file/d/1yntJz94DeGUn1oPVTqrm3-vqUdC1U0SR/preview" width="640" height="480" allow="autoplay"></iframe>

安定化電源をつかって、高い方のサーボモーターを動かそうとしたら、サーボモーターが動かなくて相談したりしました。
![image](https://github.com/user-attachments/assets/2878e18e-3ca6-45bb-ad57-52b10a809843)

詳しいメンバーが、Raspberry PiとサーボモーターのGNDに電圧差が生じて動かないことを直ぐに指摘してくれて爆速で解決しました。

送っている信号がちゃんとPWM信号になっているのか確認するため、オシロスコープを使ったりして楽しかったです。

サーボモーターを使ってチキンを鳴らすときに、お腹を押し込みすぎるとチキンのガワが凹んでしまって押し込めなくなる問題があったので、チキンの内側にペットボトルのキャップを仕込んで引っ張る仕組みを試したりしました。

![IMG_9908](https://github.com/user-attachments/assets/e49105a1-0d31-434c-98c5-3a390433866e)

<iframe src="https://drive.google.com/file/d/1OlGDO1-eT006oGun_1mGwWSx67khKF2B//preview" width="640" height="480" allow="autoplay"></iframe>

雑に試してみた割には、良い感じに動作したのでこの方式で対策しようと思います。

なんども押していると、ガワがずれていってしまう問題も残っているので、その対策も考えないといけないから大変だ～。頑張るぞ～！
