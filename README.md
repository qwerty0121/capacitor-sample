# capacitor-sample

## 概要

Vue.jsで構築したWebアプリをCapacitorを用いてネイティブアプリ化することを試す。

## 必要環境

* Node.js
* Android Studio

## 手順

1. Vue.jsでWebアプリを構築する
    ```bash
    npm init vite@latest capacitor-sample -- --template vue

    cd capacitor-sample
    npm install
    ```
1. Capacitorをインストールする
    ```bash
    npm install @capacitor/core @capacitor/cli
    npx cap init capacitor-sample com.example.capacitorsample --web-dir=dist
    ```
1. Webアプリをビルドする
    ```bash
    npm run build
    ```
1. WebアプリからAndroidアプリプロジェクトを生成する
    ```bash
    npm install @capacitor/android
    npx cap add android
    ```
1. 生成したAndroidアプリプロジェクトをAndroid Studioで開く
    ```bash
    npx cap open android
    ```
1. Android Studio上でAndroidアプリを起動する

## 参考サイト

* [モバイル | Vue.js](https://v3.ja.vuejs.org/guide/mobile.html)
* [インストール | Vue.js](https://v3.ja.vuejs.org/guide/installation.html#cli)
* [Using Capacitor with Vue - Capacitor](https://capacitorjs.com/solution/vue)
* [Capacitor Workflow](https://capacitorjs.com/docs/basics/workflow)
* [Android Studio のインストール - Mac](https://developer.android.com/studio/install?hl=ja#mac)
