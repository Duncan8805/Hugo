+++
date = 2021-04-01T14:00:00Z
title = "認識JSON"

+++

JavaScript Object Notation (JSON) 為將結構化資料 (structured data) 呈現為 JavaScript 物件的標準格式，常用於網站上的資料呈現、傳輸 (例如將資料從伺服器送至用戶端，以利顯示網頁)。你應該會常常遇到，因此本文將說明 JavaScript 搭配 JSON 時所應知道的觀念，包含如何在 JSON 物件中存取資料項目，並寫出你自己的 JSON。

JSON 可能是物件或字串。當你想從 JSON中讀取資料時，JSON可作為物件；當要跨網路傳送 JSON 時，就會是字串。這不是什麼大問題 — JavaScript 提供全域 [JSON](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON) 物件，其內的函式可進行切換。

JSON 物件可儲存於其自有的檔案中，基本上就是副檔名為 `.json` 的文字檔案，以及 `application/json` 的 [MIME type](https://developer.mozilla.org/en-US/docs/Glossary/MIME_type)。

> JSON的架構

你當然可在 JSON 之內加入相同的基本資料類型，如字串、數字、陣列、布林值，以及其他物件，接著同樣能再建構出資料繼承，如：

    {
        "title": "A",
        "post": "Test1",
        "createdate": "2021/03/17",
        "id": 1
      },
      {
        "title": "B",
        "post": "Test2",
        "createdate": "2021/03/17",
        "id": 2
      }

> 陣列的JSON

    [
      {
        "title": "A",
        "post": "Test1",
        "createdate": "2021/03/17",
        "id": 1
      },
      {
        "title": "B",
        "post": "Test2",
        "createdate": "2021/03/17",
        "id": 2
      },
      {
        "title": "C",
        "post": "Test3",
        "createdate": "2021/03/17",
        "id": 3
      },
      {
        "title": "D",
        "post": "Test4",
        "createdate": "2021/03/17",
        "id": 4
      },
      {
        "title": "E",
        "post": "Test5",
        "createdate": "2021/03/17",
        "id": 5
      },
      {
        "title": "F",
        "post": "Test6",
        "createdate": "2021/03/17",
        "id": 6
      },
      {
        "title": "G",
        "post": "Test7",
        "createdate": "2021/03/17",
        "id": 7
      }
    ]

## 參考資料

[使用JSON](https://developer.mozilla.org/zh-TW/docs/Learn/JavaScript/Objects/JSON)