# 這是什麼？

這是一個小道具，可以讓你的SCP標題整合進頁面的標題裡的同時維持原本的外觀，這樣用Listpages的時候就能直接看到你的作品名稱而不是單純的一串數字了。

# 那我該怎麼使用呢？

首先，你要透過編輯頁面把SCP的作品名稱放到標題（Title of the page）的欄位。比方說把[SCP-201]改成[SCP-201 - 空蕩蕩的世界]。

接著，根據你用的CSS不同，需要使用不一樣的代碼，不過它們都大同小異，重點是要把那一行代碼放到內容的最頂端。不過有些例外的情況，就是如果你的SCP本來就已經對標題動過一些手腳（例如[[[scp-zh-024|收容室ZH-S12-E-024實驗紀錄]]]）、[[[SCP-2998]]]（它用CSS更改了標題的顯示方式）或是你已經使用ACS標題模板（它會直接蓋過標題），那麼你可能就不需要再額外添加下列代碼。

### 無CSS（或其他Sigma-9主題）
```
[[include component:scp-meta-title-hiding css-style=classic]]
```

### 黑色標記筆（BHL）
```
[[include component:scp-meta-title-hiding css-style=bhl]]
```


### 半影（Penumbra）
```
[[include component:scp-meta-title-hiding css-style=penumbra]]
```

### 玄武岩（Basalt）
```
[[include component:scp-meta-title-hiding css-style=basalt]]
```

### 黑色玄武岩（Basalt Darkmode）
```
[[include component:scp-meta-title-hiding css-style=basalt-dark]]@@
```

### 現代外觀
※許多現代的外觀主題在一開始就已添加.meta-title的設計，因此如果你想套用的主題較新且並未列於上方，可以先嘗試這一選項的效果如何。
```
[[include component:scp-meta-title-hiding css-style=modern]]
```


## **如果您使用了Ayers的著作資訊橫幅，那麼有些標題隱藏器需要另外設置。**

### 無CSS（或其他Sigma-9主題）搭配Ayers的著作標示橫槓
```
[[include component:scp-meta-title-hiding css-style=classic-ayers]]
```

### 玄武岩（Basalt）搭配Ayers的著作標示橫槓
```
[[include component:scp-meta-title-hiding css-style=basalt-ayers]]
```

### 黑色玄武岩（Basalt Darkmode）搭配Ayers的著作標示橫槓
```
[[include component:scp-meta-title-hiding css-style=basalt-dark-ayers]]
```

# 特殊參數

以下是一些特殊狀態下可能會需要作的設定，如果不確定該如何使用的話也能到Discord聊天室詢問。

### 改變標題顏色
※可以使用 //#FFFFFF// 或 //rgb(256,256,256)// 兩種格式。
```
[[include component:scp-meta-title-hiding css-style=（如上所述）| color=標題顏色]]
```

### 自訂顯示標題
※ 通常用於填寫001提案中的標題「XXXX的提案」
※ 要注意，非001提案的SCP填寫這一格的時候，顯示出來的標題會經過處理，讓英文字母全部轉換為大寫，如果希望保持小寫的話請搭配使用下一項參數。
```
[[include component:scp-meta-title-hiding css-style=（如上所述）| showing-title=你想顯示的標題]]
```

### 解除全大寫設定
```
[[include component:scp-meta-title-hiding css-style=（如上所述）| title-transform=none]]
```

# 我一定要使用它嗎？
不一定。至少目前還沒有強制，只是我認為換過之後可以為你的作品帶來不少好處。

# 如果我想用的CSS沒有對應的版本該怎麼辦呢？
有時候確實會有這種情況，這時你可以在這一個頁面的討論區詢問看有沒有人有能力幫忙製作，或者如果你的能力足夠當然也可以自己製作。至於在標題隱藏器還沒製作出來以前，我的建議是先不要把作品名稱放上標題，畢竟「外觀」是相當重要的。

# 如果我遇到Bug怎麼辦？
請在這個頁面討論區或[*http://scp-zh-tr.wikidot.com/forum/t-14469304/#post-5195840 這一討論串]進行回報。
