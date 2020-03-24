# hexo-theme-matery

[![HitCount](http://hits.dwyl.io/blinkfox/hexo-theme-matery.svg)](http://hits.dwyl.io/blinkfox/hexo-theme-matery) [![Gitter](https://img.shields.io/gitter/room/blinkfox/hexo-theme-matery.svg)](https://gitter.im/hexo-theme-matery/Lobby?utm_source=badge) [![GitHub issues](https://img.shields.io/github/issues/blinkfox/hexo-theme-matery.svg)](https://github.com/blinkfox/hexo-theme-matery/issues) [![GitHub license](https://img.shields.io/github/license/blinkfox/hexo-theme-matery.svg)](https://github.com/blinkfox/hexo-theme-matery/blob/master/LICENSE) [![Download](https://img.shields.io/badge/downloads-master-green.svg)](https://codeload.github.com/blinkfox/hexo-theme-matery/zip/master) [![Hexo Version](https://img.shields.io/badge/hexo-%3E%3D%203.0-blue.svg)](http://hexo.io) [![GitHub forks](https://img.shields.io/github/forks/blinkfox/hexo-theme-matery.svg)](https://github.com/blinkfox/hexo-theme-matery/network) [![GitHub stars](https://img.shields.io/github/stars/blinkfox/hexo-theme-matery.svg)](https://github.com/blinkfox/hexo-theme-matery/stargazers)

[🇺🇸English Document](README.md) | [演示示例](https://blinkfox.github.io/) | QQ 交流群1（已滿）: [`926552981`](https://jq.qq.com/?_wv=1027&k=5zMDYHT) | QQ 交流群2（推薦）: [`971887688`](https://jq.qq.com/?_wv=1027&k=53q2Ayp)

> 這是一個采用 `Material Design` 和響應式設計的 Hexo 博客主題。

## 特性

- 簡單漂亮，文章內容美觀易讀
- [Material Design](https://material.io/) 設計
- 響應式設計，博客在桌面端、平板、手機等設備上均能很好的展現
- 首頁輪播文章及每天動態切換 `Banner` 圖片
- 瀑布流式的博客文章列表（文章無特色圖片時會有 `24` 張漂亮的圖片代替）
- 時間軸式的歸檔頁
- **詞雲**的標簽頁和**雷達圖**的分類頁
- 豐富的關於我頁面（包括關於我、文章統計圖、我的項目、我的技能、相冊等）
- 可自定義的數據的友情鏈接頁面
- 支持文章置頂和文章打賞
- 支持 `MathJax`
- `TOC` 目錄
- 可設置複制文章內容時追加版權信息
- 可設置閱讀文章時做密碼驗證
- [Gitalk](https://gitalk.github.io/)、[Gitment](https://imsun.github.io/gitment/)、[Valine](https://valine.js.org/) 和 [Disqus](https://disqus.com/) 評論模塊（推薦使用 `Gitalk`）
- 集成了[不蒜子統計](http://busuanzi.ibruce.info/)、谷歌分析（`Google Analytics`）和文章字數統計等功能
- 支持在首頁的音樂播放和視頻播放功能
- 支持`emoji`表情，用`markdown emoji`語法書寫直接生成對應的能**跳躍**的表情。
- 支持 [DaoVoice](http://www.daovoice.io/)、[Tidio](https://www.tidio.com/) 在線聊天功能。

## 貢獻者

感謝下面列出的貢獻者，沒有他們，hexo-theme-matery 不會這麽完美。

- [@HarborZeng](https://github.com/HarborZeng)
- [@shw2018](https://github.com/shw2018)
- [@L1cardo](https://github.com/L1cardo)
- [@Five-great](https://github.com/Five-great)

## 下載

當你看到這里的時候，應該已經有一個自己的 [Hexo](https://hexo.io/zh-cn/) 博客了。如果還沒有的話，不妨使用 Hexo 和 [Markdown](https://www.appinn.com/markdown/) 來寫博客和文章。

點擊 [這里](https://codeload.github.com/blinkfox/hexo-theme-matery/zip/master) 下載 `master` 分支的最新穩定版的代碼，解壓縮後，將 `hexo-theme-matery` 的文件夾複制到你 Hexo 的 `themes` 文件夾中即可。

當然你也可以在你的 `themes` 文件夾下使用 `Git clone` 命令來下載:

```bash
git clone https://github.com/blinkfox/hexo-theme-matery.git
```

## 配置

### 切換主題

修改 Hexo 根目錄下的 `_config.yml` 的  `theme` 的值：`theme: hexo-theme-matery`

#### `_config.yml` 文件的其它修改建議:

- 請修改 `_config.yml` 的 `url` 的值為你的網站主 `URL`（如：`http://xxx.github.io`）。
- 建議修改兩個 `per_page` 的分頁條數值為 `6` 的倍數，如：`12`、`18` 等，這樣文章列表在各個屏幕下都能較好的顯示。
- 如果你是中文用戶，則建議修改 `language` 的值為 `zh-CN`。

### 新建分類 categories 頁

`categories` 頁是用來展示所有分類的頁面，如果在你的博客 `source` 目錄下還沒有 `categories/index.md` 文件，那麽你就需要新建一個，命令如下：

```bash
hexo new page "categories"
```

編輯你剛剛新建的頁面文件 `/source/categories/index.md`，至少需要以下內容：

```yaml
---
title: categories
date: 2018-09-30 17:25:30
type: "categories"
layout: "categories"
---
```

### 新建標簽 tags 頁

`tags` 頁是用來展示所有標簽的頁面，如果在你的博客 `source` 目錄下還沒有 `tags/index.md` 文件，那麽你就需要新建一個，命令如下：

```bash
hexo new page "tags"
```

編輯你剛剛新建的頁面文件 `/source/tags/index.md`，至少需要以下內容：

```yaml
---
title: tags
date: 2018-09-30 18:23:38
type: "tags"
layout: "tags"
---
```

### 新建關於我 about 頁

`about` 頁是用來展示**關於我和我的博客**信息的頁面，如果在你的博客 `source` 目錄下還沒有 `about/index.md` 文件，那麽你就需要新建一個，命令如下：

```bash
hexo new page "about"
```

編輯你剛剛新建的頁面文件 `/source/about/index.md`，至少需要以下內容：

```yaml
---
title: about
date: 2018-09-30 17:25:30
type: "about"
layout: "about"
---
```

### 新建留言板 contact 頁（可選的）

`contact` 頁是用來展示**留言板**信息的頁面，如果在你的博客 `source` 目錄下還沒有 `contact/index.md` 文件，那麽你就需要新建一個，命令如下：

```bash
hexo new page "contact"
```

編輯你剛剛新建的頁面文件 `/source/contact/index.md`，至少需要以下內容：

```yaml
---
title: contact
date: 2018-09-30 17:25:30
type: "contact"
layout: "contact"
---
```

> **註**：本留言板功能依賴於第三方評論系統，請**激活**你的評論系統才有效果。並且在主題的 `_config.yml` 文件中，第 `19` 至 `21` 行的“**菜單**”配置，取消關於留言板的註釋即可。

### 新建友情鏈接 friends 頁（可選的）

`friends` 頁是用來展示**友情鏈接**信息的頁面，如果在你的博客 `source` 目錄下還沒有 `friends/index.md` 文件，那麽你就需要新建一個，命令如下：

```bash
hexo new page "friends"
```

編輯你剛剛新建的頁面文件 `/source/friends/index.md`，至少需要以下內容：

```yaml
---
title: friends
date: 2018-12-12 21:25:30
type: "friends"
layout: "friends"
---
```

同時，在你的博客 `source` 目錄下新建 `_data` 目錄，在 `_data` 目錄中新建 `friends.json` 文件，文件內容如下所示：

```json
[{
    "avatar": "http://image.luokangyuan.com/1_qq_27922023.jpg",
    "name": "碼醬",
    "introduction": "我不是大佬，只是在追尋大佬的腳步",
    "url": "http://luokangyuan.com/",
    "title": "前去學習"
}, {
    "avatar": "http://image.luokangyuan.com/4027734.jpeg",
    "name": "閃爍之狐",
    "introduction": "編程界大佬，技術牛，人還特別好，不懂的都可以請教大佬",
    "url": "https://blinkfox.github.io/",
    "title": "前去學習"
}, {
    "avatar": "http://image.luokangyuan.com/avatar.jpg",
    "name": "ja_rome",
    "introduction": "平凡的腳步也可以走出偉大的行程",
    "url": "https://me.csdn.net/jlh912008548",
    "title": "前去學習"
}]
```

### 菜單導航配置

#### 配置基本菜單導航的名稱、路徑url和圖標icon.

1.菜單導航名稱可以是中文也可以是英文(如：`Index`或`主頁`) 
2.圖標icon 可以在[Font Awesome](https://fontawesome.com/icons) 中查找   

```yaml
menu:
  Index:
    url: /
    icon: fas fa-home
  Tags:
    url: /tags
    icon: fas fa-tags
  Categories:
    url: /categories
    icon: fas fa-bookmark
  Archives:
    url: /archives
    icon: fas fa-archive
  About:
    url: /about
    icon: fas fa-user-circle
  Friends:
    url: /friends
    icon: fas fa-address-book
```

#### 二級菜單配置方法
如果你需要二級菜單則可以在原基本菜單導航的基礎上如下操作     
1.在需要添加二級菜單的一級菜單下添加`children`關鍵字(如:`About`菜單下添加`children`)     
2.在`children`下創建二級菜單的 名稱name,路徑url和圖標icon.      
3.註意每個二級菜單模塊前要加 `-`.     
4.註意縮進格式  

```yaml
menu:
  Index:
    url: /
    icon: fas fa-home
  Tags:
    url: /tags
    icon: fas fa-tags
  Categories:
    url: /categories
    icon: fas fa-bookmark
  Archives:
    url: /archives
    icon: fas fa-archive
  About:
    url: /about
    icon: fas fa-user-circle-o
  Friends:
    url: /friends
    icon: fas fa-address-book
  Medias:
    icon: fas fa-list
    children:
      - name: Musics
        url: /musics
        icon: fas fa-music
      - name: Movies
        url: /movies
        icon: fas fa-film
      - name: Books
        url: /books
        icon: fas fa-book
      - name: Galleries
        url: /galleries
        icon: fas fa-image
```

執行 `hexo clean && hexo g` 重新生成博客文件，然後就可以在文章中對應位置看到你用`emoji`語法寫的表情了。

### 代碼高亮

由於 Hexo 自帶的代碼高亮主題顯示不好看，所以主題中使用到了 [hexo-prism-plugin](https://github.com/ele828/hexo-prism-plugin) 的 Hexo 插件來做代碼高亮，安裝命令如下：

```bash
npm i -S hexo-prism-plugin
```

然後，修改 Hexo 根目錄下 `_config.yml` 文件中 `highlight.enable` 的值為 `false`，並新增 `prism` 插件相關的配置，主要配置如下：

```yaml
highlight:
  enable: false

prism_plugin:
  mode: 'preprocess'    # realtime/preprocess
  theme: 'tomorrow'
  line_number: false    # default false
  custom_css:
```

### 搜索

本主題中還使用到了 [hexo-generator-search](https://github.com/wzpan/hexo-generator-search) 的 Hexo 插件來做內容搜索，安裝命令如下：

```bash
npm install hexo-generator-search --save
```

在 Hexo 根目錄下的 `_config.yml` 文件中，新增以下的配置項：

```yaml
search:
  path: search.xml
  field: post
```

### 中文鏈接轉拼音（建議安裝）

如果你的文章名稱是中文的，那麽 Hexo 默認生成的永久鏈接也會有中文，這樣不利於 `SEO`，且 `gitment` 評論對中文鏈接也不支持。我們可以用 [hexo-permalink-pinyin](https://github.com/viko16/hexo-permalink-pinyin) Hexo 插件使在生成文章時生成中文拼音的永久鏈接。

安裝命令如下：

```bash
npm i hexo-permalink-pinyin --save
```

在 Hexo 根目錄下的 `_config.yml` 文件中，新增以下的配置項：

```yaml
permalink_pinyin:
  enable: true
  separator: '-' # default: '-'
```

> **註**：除了此插件外，[hexo-abbrlink](https://github.com/rozbo/hexo-abbrlink) 插件也可以生成非中文的鏈接。

### 文章字數統計插件（建議安裝）

如果你想要在文章中顯示文章字數、閱讀時長信息，可以安裝 [hexo-wordcount](https://github.com/willin/hexo-wordcount)插件。

安裝命令如下：

```bash
npm i --save hexo-wordcount
```

然後只需在本主題下的 `_config.yml` 文件中，將各個文章字數相關的配置激活即可：

```yaml
postInfo:
  date: true
  update: false
  wordCount: false # 設置文章字數統計為 true.
  totalCount: false # 設置站點文章總字數統計為 true.
  min2read: false # 閱讀時長.
  readCount: false # 閱讀次數.
```

### 添加emoji表情支持（可選的）

本主題新增了對`emoji`表情的支持，使用到了 [hexo-filter-github-emojis](https://npm.taobao.org/package/hexo-filter-github-emojis) 的 Hexo 插件來支持 `emoji`表情的生成，把對應的`markdown emoji`語法（`::`,例如：`:smile:`）轉變成會跳躍的`emoji`表情，安裝命令如下：

```bash
npm install hexo-filter-github-emojis --save
```

在 Hexo 根目錄下的 `_config.yml` 文件中，新增以下的配置項：

```yaml
githubEmojis:
  enable: true
  className: github-emoji
  inject: true
  styles:
  customEmojis:
```

### 添加 RSS 訂閱支持（可選的）

本主題中還使用到了 [hexo-generator-feed](https://github.com/hexojs/hexo-generator-feed) 的 Hexo 插件來做 `RSS`，安裝命令如下：

```bash
npm install hexo-generator-feed --save
```

在 Hexo 根目錄下的 `_config.yml` 文件中，新增以下的配置項：

```yaml
feed:
  type: atom
  path: atom.xml
  limit: 20
  hub:
  content:
  content_limit: 140
  content_limit_delim: ' '
  order_by: -date
```

執行 `hexo clean && hexo g` 重新生成博客文件，然後在 `public` 文件夾中即可看到 `atom.xml` 文件，說明你已經安裝成功了。

### 添加 [DaoVoice](http://www.daovoice.io/) 在線聊天功能（可選的）

前往 [DaoVoice](http://www.daovoice.io/) 官網註冊並且獲取 `app_id`，並將 `app_id` 填入主題的 `_config.yml` 文件中。

### 添加 [Tidio](https://www.tidio.com/) 在線聊天功能（可選的）

前往 [Tidio](https://www.tidio.com/) 官網註冊並且獲取 `Public Key`，並將 `Public Key` 填入主題的 `_config.yml` 文件中。

### 修改頁腳

頁腳信息可能需要做定制化修改，而且它不便於做成配置信息，所以可能需要你自己去再修改和加工。修改的地方在主題文件的 `/layout/_partial/footer.ejs` 文件中，包括站點、使用的主題、訪問量等。

### 修改社交鏈接

在主題的 `_config.yml` 文件中，默認支持 `QQ`、`GitHub` 和郵箱等的配置，你可以在主題文件的 `/layout/_partial/social-link.ejs` 文件中，新增、修改你需要的社交鏈接地址，增加鏈接可參考如下代碼：

```html
<% if (theme.socialLink.github) { %>
    <a href="<%= theme.socialLink.github %>" class="tooltipped" target="_blank" data-tooltip="訪問我的GitHub" data-position="top" data-delay="50">
        <i class="fab fa-github"></i>
    </a>
<% } %>
```

其中，社交圖標（如：`fa-github`）你可以在 [Font Awesome](https://fontawesome.com/icons) 中搜索找到。以下是常用社交圖標的標識，供你參考：

- Facebook: `fab fa-facebook`
- Twitter: `fab fa-twitter`
- Google-plus: `fab fa-google-plus`
- Linkedin: `fab fa-linkedin`
- Tumblr: `fab fa-tumblr`
- Medium: `fab fa-medium`
- Slack: `fab fa-slack`
- Sina Weibo: `fab fa-weibo`
- Wechat: `fab fa-weixin`
- QQ: `fab fa-qq`
- Zhihu: `fab fa-zhihu`

> **註意**: 本主題中使用的 `Font Awesome` 版本為 `5.11.0`。

### 修改打賞的二維碼圖片

在主題文件的 `source/medias/reward` 文件中，你可以替換成你的的微信和支付寶的打賞二維碼圖片。

### 配置音樂播放器（可選的）

要支持音樂播放，在主題的 `_config.yml` 配置文件中激活music配置即可：

```yaml
# 是否在首頁顯示音樂
music:
  enable: true
  title:     	    #非吸底模式有效
    enable: true
    show: 聽聽音樂
  server: netease   #require music platform: netease, tencent, kugou, xiami, baidu
  type: playlist    #require song, playlist, album, search, artist
  id: 503838841     #require song id / playlist id / album id / search keyword
  fixed: false      # 開啟吸底模式
  autoplay: false   # 是否自動播放
  theme: '#42b983'
  loop: 'all'       # 音頻循環播放, 可選值: 'all', 'one', 'none'
  order: 'random'   # 音頻循環順序, 可選值: 'list', 'random'
  preload: 'auto'   # 預加載，可選值: 'none', 'metadata', 'auto'
  volume: 0.7       # 默認音量，請註意播放器會記憶用戶設置，用戶手動設置音量後默認音量即失效
  listFolded: true  # 列表默認折疊
```

> `server`可選`netease`（網易雲音樂），`tencent`（QQ音樂），`kugou`（酷狗音樂），`xiami`（蝦米音樂），
>
> `baidu`（百度音樂）。
>
> `type`可選`song`（歌曲），`playlist`（歌單），`album`（專輯），`search`（搜索關鍵字），`artist`（歌手）
>
> `id`獲取示例: 瀏覽器打開網易雲音樂，點擊我喜歡的音樂歌單，地址欄有一串數字，`playlist`的`id`即為這串數字。



## 文章 Front-matter 介紹

### Front-matter 選項詳解

`Front-matter` 選項中的所有內容均為**非必填**的。但我仍然建議至少填寫 `title` 和 `date` 的值。

| 配置選項   | 默認值                      | 描述                                                         |
| ---------- | --------------------------- | ------------------------------------------------------------ |
| title      | `Markdown` 的文件標題        | 文章標題，強烈建議填寫此選項                                 |
| date       | 文件創建時的日期時間          | 發布時間，強烈建議填寫此選項，且最好保證全局唯一             |
| author     | 根 `_config.yml` 中的 `author` | 文章作者                                                     |
| img        | `featureImages` 中的某個值   | 文章特征圖，推薦使用圖床(騰訊雲、七牛雲、又拍雲等)來做圖片的路徑.如: `http://xxx.com/xxx.jpg` |
| top        | `true`                      | 推薦文章（文章是否置頂），如果 `top` 值為 `true`，則會作為首頁推薦文章 |
| cover      | `false`                     | `v1.0.2`版本新增，表示該文章是否需要加入到首頁輪播封面中 |
| coverImg   | 無                          | `v1.0.2`版本新增，表示該文章在首頁輪播封面需要顯示的圖片路徑，如果沒有，則默認使用文章的特色圖片 |
| password   | 無                          | 文章閱讀密碼，如果要對文章設置閱讀驗證密碼的話，就可以設置 `password` 的值，該值必須是用 `SHA256` 加密後的密碼，防止被他人識破。前提是在主題的 `config.yml` 中激活了 `verifyPassword` 選項 |
| toc        | `true`                      | 是否開啟 TOC，可以針對某篇文章單獨關閉 TOC 的功能。前提是在主題的 `config.yml` 中激活了 `toc` 選項 |
| mathjax    | `false`                     | 是否開啟數學公式支持 ，本文章是否開啟 `mathjax`，且需要在主題的 `_config.yml` 文件中也需要開啟才行 |
| summary    | 無                          | 文章摘要，自定義的文章摘要內容，如果這個屬性有值，文章卡片摘要就顯示這段文字，否則程序會自動截取文章的部分內容作為摘要 |
| categories | 無                          | 文章分類，本主題的分類表示宏觀上大的分類，只建議一篇文章一個分類 |
| tags       | 無                          | 文章標簽，一篇文章可以多個標簽                              |
| keywords   | 文章標題                     | 文章關鍵字，SEO 時需要                              |
| reprintPolicy | cc_by                    | 文章轉載規則， 可以是 cc_by, cc_by_nd, cc_by_sa, cc_by_nc, cc_by_nc_nd, cc_by_nc_sa, cc0, noreprint 或 pay 中的一個 |

> **註意**:
> 1. 如果 `img` 屬性不填寫的話，文章特色圖會根據文章標題的 `hashcode` 的值取余，然後選取主題中對應的特色圖片，從而達到讓所有文章都的特色圖**各有特色**。
> 2. `date` 的值盡量保證每篇文章是唯一的，因為本主題中 `Gitalk` 和 `Gitment` 識別 `id` 是通過 `date` 的值來作為唯一標識的。
> 3. 如果要對文章設置閱讀驗證密碼的功能，不僅要在 Front-matter 中設置采用了 SHA256 加密的 password 的值，還需要在主題的 `_config.yml` 中激活了配置。有些在線的 SHA256 加密的地址，可供你使用：[開源中國在線工具](http://tool.oschina.net/encrypt?type=2)、[chahuo](http://encode.chahuo.com/)、[站長工具](http://tool.chinaz.com/tools/hash.aspx)。
> 4. 您可以在文章md文件的 front-matter 中指定 reprintPolicy 來給單個文章配置轉載規則

以下為文章的 `Front-matter` 示例。

### 最簡示例

```yaml
---
title: typora-vue-theme主題介紹
date: 2018-09-07 09:25:00
---
```

### 最全示例

```yaml
---
title: typora-vue-theme主題介紹
date: 2018-09-07 09:25:00
author: 趙奇
img: /source/images/xxx.jpg
top: true
cover: true
coverImg: /images/1.jpg
password: 8d969eef6ecad3c29a3a629280e686cf0c3f5d5a86aff3ca12020c923adc6c92
toc: false
mathjax: false
summary: 這是你自定義的文章摘要內容，如果這個屬性有值，文章卡片摘要就顯示這段文字，否則程序會自動截取文章的部分內容作為摘要
categories: Markdown
tags:
  - Typora
  - Markdown
---
```

## 效果截圖

![首頁](http://static.blinkfox.com/matery-20181202-1.png)

![首頁推薦文章](http://static.blinkfox.com/matery-20181202-2.png)

![首頁文章列表](http://static.blinkfox.com/matery-20181202-3.png)

![首頁文章列表](http://static.blinkfox.com/matery-20181202-7.png)

![首頁文章列表](http://static.blinkfox.com/matery-20181202-8.png)

## 自定制修改

在本主題的 `_config.yml` 中可以修改部分自定義信息，有以下幾個部分：

- 菜單
- 我的夢想
- 首頁的音樂播放器和視頻播放器配置
- 是否顯示推薦文章名稱和按鈕配置
- `favicon` 和 `Logo`
- 個人信息
- TOC 目錄
- 文章打賞信息
- 複制文章內容時追加版權信息
- MathJax
- 文章字數統計、閱讀時長
- 點擊頁面的'愛心'效果
- 我的項目
- 我的技能
- 我的相冊
- `Gitalk`、`Gitment`、`Valine` 和 `disqus` 評論配置
- [不蒜子統計](http://busuanzi.ibruce.info/)和谷歌分析（`Google Analytics`）
- 默認特色圖的集合。當文章沒有設置特色圖時，本主題會根據文章標題的 `hashcode` 值取余，來選擇展示對應的特色圖

**我認為個人博客應該都有自己的風格和特色**。如果本主題中的諸多功能和主題色彩你不滿意，可以在主題中自定義修改，很多更自由的功能和細節點的修改難以在主題的 `_config.yml` 中完成，需要修改源代碼才來完成。以下列出了可能對你有用的地方：

### 修改主題顏色

在主題文件的 `/source/css/matery.css` 文件中，搜索 `.bg-color` 來修改背景顏色：

```css
/* 整體背景顏色，包括導航、移動端的導航、頁尾、標簽頁等的背景顏色. */
.bg-color {
    background-image: linear-gradient(to right, #4cbf30 0%, #0f9d58 100%);
}

@-webkit-keyframes rainbow {
   /* 動態切換背景顏色. */
}

@keyframes rainbow {
    /* 動態切換背景顏色. */
}
```

### 修改 banner 圖和文章特色圖

你可以直接在 `/source/medias/banner` 文件夾中更換你喜歡的 `banner` 圖片，主題代碼中是每天動態切換一張，只需 `7` 張即可。如果你會 `JavaScript` 代碼，可以修改成你自己喜歡切換邏輯，如：隨機切換等，`banner` 切換的代碼位置在 `/layout/_partial/bg-cover-content.ejs` 文件的 `<script></script>` 代碼中：

```javascript
$('.bg-cover').css('background-image', 'url(/medias/banner/' + new Date().getDay() + '.jpg)');
```

在 `/source/medias/featureimages` 文件夾中默認有 24 張特色圖片，你可以再增加或者減少，並需要在 `_config.yml` 做同步修改。

## 版本記錄

- v1.2.2
  - 新增了自定義文章 `keywords` 的功能；
  - 新增靜態彩帶點擊切換的功能和配置；
  - 將文章字數統計、彩帶和站點運行時間等功能默認設置為 `false`；
  - 修改了文章的 `description` 的 meta 屬性優先讀取文章的 `summary` 屬性；
  - 修改了文章標題的 HTML 標簽，從 `div` 改成了 `h1` 標題；
  - 修改了頁腳年份顯示不正確的問題；
  - 去掉了站點運行時間中多余的 `setTimeout` 代碼；
- v1.2.1
  - 新增了 TOC 的展開目錄層級設置和滾動條功能，防止目錄較多的時候目錄溢出；
  - 修改了首頁的展示方式為以前的模式；
  - 修複首頁按鈕沒有邊框的問題；
  - 修複了音樂及吸底模式、視頻、推薦文章等不激活時仍然生成首頁卡片的問題；
  - 修複 wordCount 插件未安裝的問題，修改了部分配置；
  - 修複音樂的 JSON 配置中有單引號的情況頁面不顯示的音樂的問題
  - 修複標簽雲在Hexo4.0下鏈接失效的問題；
- v1.2.0
  - 新增了 [DaoVoice](http://www.daovoice.io/)、[Tidio](https://www.tidio.com/) 的在線聊天功能；
  - 新增了兩級菜單的功能；
  - 新增了打字效果的副標題；
  - 新增了網頁內容預加載的功能；
  - 新增了首頁 banner 是否每日切換的配置功能；
  - 新增了顯示 ICP 備案信息的功能，默認未開啟；
  - 新增了百度分析的配置；
  - 新增了代碼塊的語言顯示、一鍵複制、顯示行號等功能；
  - 新增了首頁輪播圖和推薦文章可自定義配置的功能；
  - 新增了文章頁面顯示更新日期；
  - 新增了轉載規則的圖標；
  - 修改了分享的布局和顯示方式；
  - 升級更新了部分依賴庫的版本；
  - 其他細節修改和優化；
- v1.1.0
  - 新增了 `emoji` 的支持；
  - 新增了站點運行時間統計及配置；
  - 新增了留言板的功能,默認未開啟；
  - 新增了 `Twitter`、`Facebook`、知乎的社交鏈接；
  - 更新了 `Valine` 的版本為最新版；
  - 其他小細節的修改；
- v1.0.4
  - 新增了能為每篇文章都自定義轉載規則的功能；
  - 修複上一頁、下一頁的自定義 `summary` 不顯示的問題；
  - 修複了友情鏈接顯示錯位的問題，改為了瀑布流的布局方式；
  - 其他小細節 bug 的修改；
- v1.0.3
  - 新增了`TOC`展開、收縮的按鈕和相關配置，默認顯示此按鈕；
- v1.0.2
  - 升級了 [Materialize](https://materializecss.com/) 框架版本為`1.0.0`，重構和修改了升級過程中的部分文件或問題；
  - 新增了首頁封面的全屏輪播特效，可以將更重要的文章設置到首頁輪播中；
  - 修複首頁第一個按鈕是中文的問題
  - 修複了 iPhone 上點擊搜索輸入獲取焦點的問題；
  - 修複了 iPhone 上輸入框獲取焦點後頁面放大的問題；
  - 修複一些文章或 UI 顯示問題；
- v1.0.1
  - 調整 `css`、`js` 的文件請求路徑在主題的`_config.yml`中配置，便於你更快捷的配置自己的 CDN；
  - 新增代碼是否折行為可配置，默認為折行；
  - 默認激活 `TOC` 功能，並新增為某篇文章關閉 `TOC` 的 `Front-matter` 配置選項；
  - 修複文章滾動時，高亮的目錄選項不準確的問題；
  - `IOS`下移除搜索框自動獲得焦點屬性，防止自動獲得焦點後導致視圖上移；
- v1.0.0
  - 新增了所有基礎功能；
