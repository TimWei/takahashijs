#高橋流簡報JS#

<a href='https://timwei.github.io/takahashijs/'><h3>DEMO</h3></a>
<a href='https://www.youtube.com/watch?v=Vor6Yul7CMg'><h5>高橋簡報現場(視頻)</h5></a>
---

### 如何使用 ###
依賴於VueJS

可直接修改數據，增減投影片數量與修改內容

</br>
<b>1. 新增投影片</b>
```
	var page_data = [
		{content: [''], header: '', footer: ''},
	];
```

如果要新增投影片時，只要新增page_data陣列內的元素

例如想產生三張投影片，只要將代碼改為

```javascript
		var page_data = [
			{content: [''], header: '', footer: ''},
			{content: [''], header: '', footer: ''},
			{content: [''], header: '', footer: ''},
		];
```

這個陣列每個元素都會是一張投影片

content可以放入 
* 字串
* 圖片鏈接

```javascript
	['first_string second_string third_string']
```
會產生一行'first_string second_string third_string'的投影片，
```javascript
	['first_string','second_string','third_string']
```
會產生分三行的投影片

header與footer內為字串，會在上方與下方產生紅字

不建議一張圖片放置超過四行的高度

</br>
<b>2. APP視圖</b>

```javascript
	<div class='taka_hashi'>
		<taka-arrow></taka-arrow>
		<taka-content></taka-content>
		<taka-fs></taka-fs>
	</div>
```

可以自行定義組件後，於此拆裝

</br>
### 特色 ###
* 文字簡單</br>
* 發表容易</br>
* 幽默、適合社群簡報</br>


</br>
### 功能 ###
* 數據產生投影片</br>
* 組件式結構，可以輕鬆修改APP組件</br>
* 點擊投影片右方會撥放下一張，左方撥放前一張</br>
* 可用方向鍵或空白、回車鍵操控</br>
* 預設組件右下角有全屏按鈕，可以做出類似PPT的投影片播放</br>

</br>
### 結構 ###
* 將結構為{content: ['頭影片內容'], header: '上標文字', footer: '下標文字'}放入陣列，即可產生投影片

---

</br>
### 誰是高橋? ###
* 日本Ruby協會會長
* 翻譯了Ruby的中文書
* <b>製作性價比極高的簡報</b>


