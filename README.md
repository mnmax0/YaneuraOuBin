LaTeX:t \^:{}

YaneuraOuさんの将棋エンジンAndroid arm64-v8a向けバイナリ
========================================================

id 9bbd0f38498b22e9f3e6cf9493a7f8849c02e496 からコンパイル

将棋エンジンのコンパイルの時に使っているコマンド
================================================

``` {.bash}
ndk-build TARGET_ARCH_ABI=arm64-v8a clean
ndk-build TARGET_ARCH_ABI=arm64-v8a 2>&1 | tee log_android_nn001.txt
```

-   バイナリのファイル名  YaneuraOu\_NNUE\_arm64-v8a
-   コンパイル時のログ  log\_android\_nn001.txt

詰将棋将棋エンジンのコンパイルの時に使っているコマンド
======================================================

``` {.bash}
ndk-build YANEURAOU_EDITION=TANUKI_MATE_ENGINE TARGET_ARCH_ABI=arm64-v8a ENGINE_NAME=Tanuki_MATE_arm64-v8a  clean
ndk-build YANEURAOU_EDITION=TANUKI_MATE_ENGINE TARGET_ARCH_ABI=arm64-v8a ENGINE_NAME=Tanuki_MATE_arm64-v8a  2>&1 | tee log_tanukimate001.txt
```

-   バイナリのファイル名  Tanuki\_MATE\_arm64-v8a\_arm64-v8a
-   コンパイル時のログ log\_tanukimate001.txt

ソースファイル名
================

-   YaneuraOu\_年月日\_時間分\_000.tgz
    -   例  YaneuraOu\_20210605\_0602\_000.tgz
-   以下のコマンドで作成

``` {.bash}
DT=`date +%Y%m%d_%H%M`
git clone https://github.com/yaneurao/YaneuraOu.git
tar cvzf YaneuraOu_${DT}_000.tgz YaneuraOu/
```

