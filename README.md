Welcome to TableForm
===================

#### **簡單好用，一份以原生Table進行排版的表單UI。**

哈囉! TableForm單純直覺只為自已的便利而誕生，快速建立聯絡表單，如果你也需要歡迎將它收到你的工具箱裡。

### [<i class="icon-download"></i> TableForm Download][0]
----------

文件檔案
-------------

考慮到了視覺設定上的彈性，提供了 **SASS** 檔及可以快速產出html格式的 [Sublime text 的程式碼片段](#html-格式-snippet)，你當然也可以直接使用css檔 :

> - tableform.css
> - tableform.scss
> - <i class="icon-folder"> snippets
>  -  tableform-html.sublime-snippet
>  -  tableform-radio.sublime-snippet
>  -  tableform-button.sublime-snippet

如何使用
------------

> 1. 下載 **tableform.scss** 放到你 **sass** 的開發資料夾
> 2. @import " tableform.scss";
> 3. 設定 `樣式主色` 或 `樣式前綴` [請參照 SASS 樣式變數對照](#sass-樣式變數對照)

----

### HTML 格式 Snippet


|                  | 標籤                        | 標籤觸發              |
 ----------------- | ---------------------------- | ------------------
| 完整表單  		  | `table`            | `tableform` |
| 表頭		  | `th`           | `-` |
| 表格標題  		  | `cpation`            | `-` |
| 下拉選單  		  | `select`            | `-` |
| 單選框  		  | `input[type=radio]`            | `radio(tbf)` |
| 按鈕組  		  | `button[type=cancel]`            | `button(tbf)` |



----

### SASS 樣式變數對照

在 [Sass][1] 裡使用了 [compass][2]，讓樣式設定方便許多，你可以先設定一個基色，再以利用compass提供的mixin，如: darken、lighten.......等，直接使用基色去做顏色的調亮或調暗，相當方便也利於管理。

> **<i class="icon-doc"></i> 提醒 tableform.scss**   //   @import "compass";

|                  | 變數                        | 預設值              |
 ----------------- | ---------------------------- | ------------------
| 樣式前綴		  | `tbf_prefix`           | `'.tbf-'` |
| 樣式主色  		  | `tbf_theme`            | `#4fa1db` |
| 表格標題文字顏色		  | `tbf_cap_txt`			| `$tbf_theme` |
| 表格標題下邊框顏色		  | `tbf_cap_border`			| `$tbf_theme` |
| 表格文字顏色 	  | `tbf_txt`		| `#ccc` |
| 表頭文字顏色 	  | `tbf_th_txt`		| `darken($tbf_txt, 40%)` |
| 表格輸入框、選擇框文字顏色 	  | `tbf_type_txt`		| `lighten($tbf_theme, 10%)` |
| 表格輸入框、選擇框邊框顏色 	  | `tbf_type_border`		| `$tbf_theme` |
| 單選框邊框顏色 	  | `tbf_radio_border`		| `$tbf_theme` |
| 單選框填滿顏色 	  | `tbf_radio_fill`		| `$tbf_theme` |
| 佔位符文字顏色 	  | `tbf_placeholder_txt`		| `lighten(#bfbfbf, 5%)` |
| 按鈕文字顏色		  | `tbf_btn_txt`			| `#fff` |
| 送出按鈕顏色		  | `tbf_btn_bgA`			| `$tbf_theme` |
| 取消按鈕顏色		  | `tbf_btn_bgB`			| `#ddd` |

基本上只要更改樣式主色就可以了，因為大多顏色基色都是來自主色，除非你有特別的配色方案，那麼你可以盡情的利用這些變數細項，來調配出多種的色彩方案。

----

#### <i class="icon-pencil"></i> DEMO

[<i class="icon-download"></i> TableForm Demo][3]


----------


> **授權說明:**

> - 隨意你使用，只要喜歡請將它帶走並使用在任何產品物件上。

----
  [0]: https://github.com/Crackccc/tableform/archive/master.zip "TableForm"
  [1]: http://sass-lang.com/ "Sass"
  [2]: http://compass-style.org/ "Compass"
  [3]: http://www.31webdesign.com/lab_tableform/ "TableForm Demo"
