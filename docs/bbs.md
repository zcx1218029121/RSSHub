---
pageClass: routes
---

# 论坛

## A 岛匿名版

### 串

<Route author="zcx1218029121" example="/adnmb/20/1" path="/adnmb/:pid/page" :paramsDesc="['板块列表，见下表','页数， 1开始必填']" >

| 综合版 1 | 围炉 | 欢乐恶搞 | 速报 2 | 推理 | 跑团 | 技术宅 | 料理 | 猫版 | 音乐 | 考试 | 社畜 |
| -------- | ---- | -------- | ------ | ---- | ---- | ------ | ---- | ---- | ---- | ---- | ---- |
| 4        | 120  | 20       | 121    | 11   | 111  | 30     | 32   | 40   | 35   | 56   | 110  |

| 科学 | 文学 | 创意 | 姐妹 1 | 数码 | 女装 | 日记 | 圈内 | 都市怪谈 | 买买买 | 动画 | 漫画 | 美漫 | 国漫 | 小说 |
| ---- | ---- | ---- | ------ | ---- | ---- | ---- | ---- | -------- | ------ | ---- | ---- | ---- | ---- | ---- |
| 15   | 103  | 17   | 98     | 75   | 97   | 89   | 96   | 81       | 106    | 14   | 12   | 90   | 99   | 19   |

| 轻小说 | GALGAME | 东方 Project | 舰娘 | 虚拟偶像 | VOCALOID | 游戏 | DNF | SE  | 手游 |
| ------ | ------- | ------------ | ---- | -------- | -------- | ---- | --- | --- | ---- |
| 87     | 64      | 5            | 93   | 101      | 6        | 2    | 72  | 124 | 3    |

| Steam | 索尼 | LOL | DOTA | 口袋妖怪 | 战争雷霆 | WOT | Minecraft | 怪物猎人 | 3A 游戏 |
| ----- | ---- | --- | ---- | -------- | -------- | --- | --------- | -------- | ------- |
| 107   | 24   | 22  | 70   | 38       | 86       | 51  | 10        | 28       | 108     |

| 彩虹六号 | 暴雪游戏 | 卡牌桌游 | MUG | AC 大逃杀 | 任天堂 | AKB | SNH48 | COSPLAY | 声优 |
| -------- | -------- | -------- | --- | --------- | ------ | --- | ----- | ------- | ---- |
| 119      | 23       | 45       | 34  | 29        | 25     | 16  | 100   | 13      | 55   |

| 模型 | 影视 | 军武 | 体育 | 值班室 | 城墙 | 技术支持 | 询问 3 | 宠物 | 摄影 2 |
| ---- | ---- | ---- | ---- | ------ | ---- | -------- | ------ | ---- | ------ |
| 39   | 31   | 37   | 33   | 18     | 112  | 117      | 114    | 118  | 115    |

| 主播 | 育儿 | 围炉 | 旅行 | 特摄 |
| ---- | ---- | ---- | ---- | ---- |
| 116  | 113  | 120  | 125  | 9    |

</Route>

## Chiphell

### 子版块

<Route author="tylinux" example="/chiphell/forum/80" path="/chiphell/forum/:forumId" :paramsDesc="['子版块 id，可在子版块 URL 找到']"/>

## Dcard

### 首頁帖子

<Route author="DIYgod" example="/dcard/posts/popular" path="/dcard/posts/:type?" :paramsDesc="['排序，popular 熱門；latest 最新，默認為 latest']" radar="1"/>

### 板塊帖子

<Route author="HenryQW" example="/dcard/funny/popular" path="/dcard/:section/:type?" :paramsDesc="['板塊名稱，URL 中獲得', '排序，popular 熱門；latest 最新，默認為 latest']" radar="1"/>

## Discuz

### 通用子版块-自动检测

<Route author="junfengP" example="/discuz/http%3a%2f%2fwww.u-share.cn%2fforum.php%3fmod%3dforumdisplay%26fid%3d56" path="/discuz/:link" :paramsDesc="['子版块链接， 需要手动Url编码']"/>

### 通用子版块-指定版本

<Route author="junfengP" example="/discuz/x/https%3a%2f%2fwww.52pojie.cn%2fforum-16-1.html" path="/discuz/:ver/:link" :paramsDesc="['discuz版本类型，见下表','子版块链接， 需要手动Url编码']" >

| Discuz X 系列 | Discuz 7.x 系列 |
| ------------- | --------------- |
| x             | 7               |

</Route>

### 通用子版块-支持 Cookie

<Route author="junfengP" example="/discuz/x/00/https%3a%2f%2fbbs.zdfx.net%2fforum-2-1.html" path="/discuz/:ver/:cid/:link" :paramsDesc="['discuz版本类型，见下表', 'Cookie id，需自建并配置环境变量，详情见部署页面的配置模块','子版块链接， 需要手动Url编码']" >

| Discuz X 系列 | Discuz 7.x 系列 |
| ------------- | --------------- |
| x             | 7               |

</Route>

## eTOLAND

### 主题贴

<Route author="mengx8" example="/etoland/star01" path="/etoland/:boardId" :paramsDesc="['板块 id，可在板块 URL 找到']"/>

## LearnKu

### 社区

<Route author="haokaiyang" example="/learnku/laravel/qa" path="/learnku/:community/:category?" :paramsDesc="['社区 标识，可在 <https://learnku.com/communities> 找到', '分类，如果不传 `category` 则获取全部分类']"/>

| 招聘 | 翻译         | 问答 | 链接  |
| ---- | ------------ | ---- | ----- |
| jobs | translations | qa   | links |

## MCBBS

### 版块

<Route author="cssxsh" example="/mcbbs/forum/news" path="/mcbbs/forum/:type" :paramsDesc="['版块名称或者版块号']"/>

### 帖子

<Route author="cssxsh" example="/mcbbs/post/915861/3038" path="/mcbbs/post/:tid/:authorid?" :paramsDesc="['贴子id，可在帖子 URL 找到', '用户id，此参数不为空时，只看此作者']"/>

## NGA

### 分区帖子

<Route author="xyqfer" example="/nga/forum/489" path="/nga/forum/:fid/:recommend?"  :paramsDesc="['分区 id, 可在分区主页 URL 找到, 没有 fid 时 stid 同样适用','是否只显示精华主题, 留空为否, 任意值为是']" radar="1"/>

### 帖子

<Route author="xyqfer" example="/nga/post/18449558" path="/nga/post/:tid"  :paramsDesc="['帖子 id, 可在帖子 URL 找到']" radar="1"/>

## Saraba1st

### 帖子

<Route author="zengxs" example="/saraba1st/thread/1789863" path="/saraba1st/thread/:tid" :paramsDesc="['帖子 id']">

帖子网址如果为 <https://bbs.saraba1st.com/2b/thread-1789863-1-1.html> 那么帖子 id 就是 `1789863`。

</Route>

## V2EX

### 最热/最新主题

<Route author="WhiteWorld" example="/v2ex/topics/latest" path="/v2ex/topics/:type" :paramsDesc="['hot 或 latest']"/>

### 帖子

<Route author="kt286" example="/v2ex/post/584403" path="/v2ex/post/:postid" :paramsDesc="['帖子ID，在 URL 可以找到']"/>

## 电鸭社区

### 工作机会

<Route author="sfyumi" example="/eleduck/jobs" path="/eleduck/jobs"/>

## 虎扑

### 虎扑 BBS 论坛

<Route author="LogicJake" example="/hupu/bbs/bxj/2" path="/hupu/bbs/:id/:order?" :paramsDesc="['板块 id，可在板块 URL 找到', '排序方式，1最新回帖（默认），2最新发帖，3精华帖']"/>

## 看雪

### 论坛

<Route author="renzhexigua" example="/pediy/topic/android/digest" path="/pediy/topic/:category?/:type?" :paramsDesc="['版块, 缺省为`all`', '类型, 缺省为`latest`']"/>

| 版块         | category   |
| ------------ | ---------- |
| 智能设备     | iot        |
| 区块链安全   | blockchain |
| Android 安全 | android    |
| iOS 安全     | ios        |
| 软件逆向     | re         |
| 编程技术     | coding     |
| 加壳脱壳     | unpack     |
| 密码算法     | crypto     |
| 二进制漏洞   | vuln       |
| CrackMe      | crackme    |
| Pwn          | pwn        |
| WEB 安全     | web        |
| 全站         | all        |

| 类型     | type   |
| -------- | ------ |
| 最新主题 | latest |
| 精华主题 | digest |

## 龙空

### 分区

<Route author="ma6254" example="/lkong/forum/60" path="/lkong/forum/:id/:digest?" :paramsDesc="['分区 id, 可在分区的URL里找到','默认获取全部主题，任意值则只获取精华主题']"/>

### 帖子

<Route author="ma6254" example="/lkong/thread/2356933" path="/lkong/thread/:id?" :paramsDesc="['帖子 id, 可在帖子的URL里找到']"/>

## 龙腾网

### 转译网贴

<Route author="sgqy" example="/ltaaa" path="/ltaaa/:type?" :paramsDesc="['热门类型.']">

| 最新 | 每周 | 每月  | 全年 |
| ---- | ---- | ----- | ---- |
| (空) | week | month | year |

</Route>

## 牛客网

### 讨论区

<Route author="LogicJake" example="/nowcoder/discuss/2/4" path="/nowcoder/discuss/:type/:order" :paramsDesc="['讨论区分区id 在 URL 中可以找到', '排序方式']">

| 最新回复 | 最新发表 | 最新 | 精华 |
| -------- | -------- | ---- | ---- |
| 0        | 3        | 1    | 4    |

</Route>

## 书友社区

### 导读

<Route author="AngUOI" example="/andyt/newthread" path="/andyt/:view?" :paramsDesc="['子版块 view, 为空默认最新发表']">

| 最新发表  | 最新热门 | 最新精华 | 最新回复 |
| --------- | -------- | -------- | -------- |
| newthread | hot      | digest   | new      |

</Route>

## 天涯论坛

### 子版块

<Route author="a14907" example="/tianya/index/lookout" path="/tianya/index/:type" :paramsDesc="['板块类型 type，可在 URL 找到 例如，天涯杂谈板块的地址是http://bbs.tianya.cn/list-free-1.shtml， 这个板块的type就是free; 同理，我的大学板块地址为http://bbs.tianya.cn/list-university-1.shtml，类型是university']"/>

### 用户帖子

<Route author="a14907" example="/tianya/user/11488997" path="/tianya/user/:userid" :paramsDesc="['用户id userid，可在 URL 找到 例如，用户苕木匠的地址是http://www.tianya.cn/11488997/bbs， 苕木匠的userid就是11488997']"/>

### 用户的回帖

<Route author="a14907" example="/tianya/comments/11488997" path="/tianya/comments/:userid" :paramsDesc="['用户id userid，可在 URL 找到 例如，用户苕木匠的地址是http://www.tianya.cn/11488997/bbs， 苕木匠的userid就是11488997']"/>

## 贴吧

### 帖子列表

<Route author="u3u" example="/tieba/forum/女图" path="/tieba/forum/:kw" :paramsDesc="['吧名']"/>

### 精品帖子

<Route author="u3u" example="/tieba/forum/good/女图" path="/tieba/forum/good/:kw/:cid?" :paramsDesc="['吧名', '精品分类, 如果不传 `cid` 则获取全部分类']"/>

### 帖子动态

<Route author="u3u" example="/tieba/post/5853240586" path="/tieba/post/:id" :paramsDesc="['帖子 ID']"/>

### 楼主动态

<Route author="u3u" example="/tieba/post/lz/5853240586" path="/tieba/post/lz/:id" :paramsDesc="['帖子 ID']"/>

## 小米社区

### 圈子

<Route author="DIYgod" example="/mi/bbs/board/18066617" path="/mi/bbs/board/:boardId" :paramsDesc="['圈子 id，可在圈子 URL 找到']" radar="1"/>

## 一亩三分地

### 主题帖

<Route author="Maecenas" example="/1point3acres/user/1/threads" path="/1point3acres/user/:id/threads" :paramsDesc="['用户 id，可在 Instant 版网站的个人主页 URL 找到']"/>

### 回帖

<Route author="Maecenas" example="/1point3acres/user/1/posts" path="/1point3acres/user/:id/posts" :paramsDesc="['用户 id，可在 Instant 版网站的个人主页 URL 找到']"/>

### 帖子 (手机端的最热与最新 Tab)

<Route author="NavePnow" example="/1point3acres/post/hot" path="/1point3acres/post/:category" :paramsDesc="['分类 category, 见下表']"/>

| 最热帖子 | 最新帖子 |
| -------- | -------- |
| hot      | new      |

### 录取结果

<Route author="NavePnow" example="/1point3acres/offer/12/null/CMU" path="/1point3acres/offer/:year?/:major?/:school?" :paramsDesc="['录取年份  id，空为null', '录取专业 id，空为null', '录取学校 id，空为null']">
::: warning 三个 id 获取方式

1. 打开 https://offer.1point3acres.com
2. 打开控制台
3. 切换到 Network 面板
4. 点击 搜索 按钮
5. 点击 results?ps=15&pg=1 POST 请求
6. 找到 Request Payload 请求参数，例如 filters: {planyr: "13", planmajor: "1", outname_w: "ACADIAU"} ，则三个 id 分别为: 13,1,ACADIAU

:::
</Route>

## 直播吧

### 子论坛

<Route author="LogicJake" example="/zhibo8/forum/8" path="/zhibo8/forum/:id" :paramsDesc="['子论坛 id，可在子论坛 URL 找到']"/>

### 回帖

<Route author="LogicJake" example="/zhibo8/post/2601615" path="/zhibo8/post/:id" :paramsDesc="['帖子 id，可在帖子 URL 找到']"/>

## a 岛匿名版

### 串

<Route author="zcx1218029121" example="/adnmb/20/1" path="/adnmb/:pid/page" :paramsDesc="['板块列表，见下表','页数， 1开始必填']" >

| 综合版 1 | 围炉 | 欢乐恶搞 | 速报 2 | 推理 | 跑团 | 技术宅 | 料理 | 猫版 | 音乐 | 考试 | 社畜 |
| -------- | ---- | -------- | ------ | ---- | ---- | ------ | ---- | ---- | ---- | ---- | ---- |
| 4        | 120  | 20       | 121    | 11   | 111  | 30     | 32   | 40   | 35   | 56   | 110  |

| 科学 | 文学 | 创意 | 姐妹 1 | 数码 | 女装 | 日记 | 圈内 | 都市怪谈 | 买买买 | 动画 | 漫画 | 美漫 | 国漫 | 小说 |
| ---- | ---- | ---- | ------ | ---- | ---- | ---- | ---- | -------- | ------ | ---- | ---- | ---- | ---- | ---- |
| 15   | 103  | 17   | 98     | 75   | 97   | 89   | 96   | 81       | 106    | 14   | 12   | 90   | 99   | 19   |

| 轻小说 | GALGAME | 东方 Project | 舰娘 | 虚拟偶像 | VOCALOID | 游戏 | DNF | SE  | 手游 |
| ------ | ------- | ------------ | ---- | -------- | -------- | ---- | --- | --- | ---- |
| 87     | 64      | 5            | 93   | 101      | 6        | 2    | 72  | 124 | 3    |

| Steam | 索尼 | LOL | DOTA | 口袋妖怪 | 战争雷霆 | WOT | Minecraft | 怪物猎人 | 3A 游戏 |
| ----- | ---- | --- | ---- | -------- | -------- | --- | --------- | -------- | ------- |
| 107   | 24   | 22  | 70   | 38       | 86       | 51  | 10        | 28       | 108     |

| 彩虹六号 | 暴雪游戏 | 卡牌桌游 | MUG | AC 大逃杀 | 任天堂 | AKB | SNH48 | COSPLAY | 声优 |
| -------- | -------- | -------- | --- | --------- | ------ | --- | ----- | ------- | ---- |
| 119      | 23       | 45       | 34  | 29        | 25     | 16  | 100   | 13      | 55   |

| 模型 | 影视 | 军武 | 体育 | 值班室 | 城墙 | 技术支持 | 询问 3 | 宠物 | 摄影 2 |
| ---- | ---- | ---- | ---- | ------ | ---- | -------- | ------ | ---- | ------ |
| 39   | 31   | 37   | 33   | 18     | 112  | 117      | 114    | 118  | 115    |

| 主播 | 育儿 | 围炉 | 旅行 | 特摄 |
| ---- | ---- | ---- | ---- | ---- |
| 116  | 113  | 120  | 125  | 9    |
