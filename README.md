# Q914

QCamVer-1 (旧称 CuCuCam) のボタン、高さ計測用超音波距離測定およびLED回路


## ボタン回路

２個ボタンを有して、1つはシャッター、他方はshutdownを起動する。

* SW1 - SHUTTER - GPIO23
* SW2 - SHUTDOWN - GPIO24

## LED回路

３個のLEDを有して、１つは赤色、他は緑色。LOWで点灯する。

* D1 - 緑 - GPIO04 ハートビート
* D2 - 緑 - GPIO05 撮影中点灯
* D3 - 赤 - GPIO06 未設定

## 超音波距離測定回路

HC-SR04を用いてカメラの高さを計測する。

* TRIG - GPIO17
* ECHO - GPIO27

に接続する。ECHOは抵抗分圧して5Vを3V程度にして接続する。
