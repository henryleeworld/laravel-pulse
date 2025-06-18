# Laravel 10 脈搏

引入 laravel 的 pulse 套件來擴增即時應用程式效能監控工具和儀表板，可以確保自身維持預期的服務水準，讓客戶獲得良好的應用程式體驗。

## 使用方式
- 把整個專案複製一份到你的電腦裡，這裡指的「內容」不是只有檔案，而是指所有整個專案的歷史紀錄、分支、標籤等內容都會複製一份下來。
```sh
$ git clone
```
- 將 __.env.example__ 檔案重新命名成 __.env__，如果應用程式金鑰沒有被設定的話，你的使用者 sessions 和其他加密的資料都是不安全的！
- 當你的專案中已經有 composer.lock，可以直接執行指令以讓 Composer 安裝 composer.lock 中指定的套件及版本。
```sh
$ composer install
```
- 產生 Laravel 要使用的一組 32 字元長度的隨機字串 APP_KEY 並存在 .env 內。
```sh
$ php artisan key:generate
```
- 執行 __Artisan__ 指令的 __migrate__ 來執行所有未完成的遷移。
```sh
$ php artisan migrate
```
- 在瀏覽器中輸入已定義的路由 URL 來訪問，例如：http://127.0.0.1:8000。
- 你可以經由 `/` 來瀏覽歡迎頁面；經由 `/pulse` 來進行應用程式效能監控儀表板瀏覽。

----

## 畫面截圖
![](https://i.imgur.com/MnhoqwY.png)
> 有助於確保服務平穩執行，停機時間降至最低，並確保客戶始終獲得積極的體驗
