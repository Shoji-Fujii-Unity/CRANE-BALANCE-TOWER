# SWING★STACK 3D — スイングスタック 3D | CRANE BALANCE TOWER

一本のHTMLファイルで動く、クレーンのバランスタワー積み3Dタイミングアクションゲーム。
A 3D timing-action balance game in a single HTML file.
单个 HTML 文件即可运行的起重机平衡堆叠 3D 动作游戏。

---

## 日本語

### 概要
毎回異なる揺れ方をするクレーンから、タイミングよく画面をタップしてさまざまな形のパーツを落とし、どこまで高くバランスよく積めるかを競うゲームです。PCとスマートフォンに対応し、画面は縦（9:16）レイアウトです。

### 起動方法
1. index.html をブラウザ（最新版の Chrome / Edge / Safari 推奨）で開きます。
2. Three.js と cannon-es を CDN（jsDelivr）から読み込むため、インターネット接続が必要です。
3. スマートフォンの場合は index.html を端末にコピーしてブラウザで開くと、縦画面でそのまま遊べます。

### 遊び方
- 画面タップ（PCはスペースキー / Enterキーでも可）で、クレーンがつり下げているパーツをリリースします。
- 落下したパーツを台の上のタワーに積み上げ、ステージで指定された高さまで到達させればクリアです。
- 中心軸から大きく外れた落下、床への落下はミスになり、ミスが3回で失敗です。
- 着地点がタワー中心から0.3m以内なら「PERFECT!!」ボーナスが入ります。
- クリア時の残りライフが星の成績になり、スコアとタワーの高さはステージごとに保存されます。

### 操作
- タップ / スペース / Enter：パーツを落とす
- P キー / Escキー：ポーズ（メニューに戻る）
- タイトル画面：言語切り替え（日本語 / English / 中文）、サウンド ON / OFF

### ステージ
ステージ1〜12とエンドレスモードの全13種。スイングパターンは線形・振り子・波・ドリフト・複合の5種で、毎回振幅と速度がランダムに変化します。強風ステージや重力が強いステージ、円柱・六角柱・三角柱・L型金具・ボールなど全12種類のパーツが登場します。ステージはクリアすると次のステージが解放されます。

### セーブデータ
ブラウザの localStorage（キー名 swingstack_save_v1）に、言語・サウンド設定・各ステージのクリア星数・ベストスコア・エンドレス最高高度が保存されます。削除する場合はブラウザ設定からこのサイトのデータ（サイト設定 / ストレージ）を消去してください。

### 技術
- Three.js 0.160（描画）と cannon-es 0.20（物理）を ES モジュールとして CDN 読み込み
- 効果音と BGM は WebAudio API で手続き生成（外部音声ファイルなし）
- 外部アセット不要の単一ファイル構成

---

## English

### Overview
Drop parts from a crane that swings in a different pattern every time, and compete on how high and how balanced you can build a tower. A timing-action balance game that runs on both PC and smartphone, in portrait (9:16) layout.

### How to Run
1. Open index.html in a modern browser (latest Chrome / Edge / Safari recommended).
2. Internet access is required because Three.js and cannon-es are loaded from the jsDelivr CDN.
3. On a phone, copy index.html to the device and open it in a mobile browser — it is ready to play in portrait.

### How to Play
- Tap the screen (or press Space / Enter on PC) to release the part hanging from the crane.
- Stack the falling parts on the platform tower and reach the stage's target height to clear.
- Dropping far off the tower axis or hitting the floor counts as a miss; 3 misses ends the run.
- Landing within 0.3 m of the tower's center axis awards a PERFECT!! bonus.
- Remaining lives become your star rating, and score and tower height are saved per stage.

### Controls
- Tap / Space / Enter: drop the part
- P / Esc: pause (returns to menu)
- Title screen: language switch (日本語 / English / 中文) and Sound ON / OFF

### Stages
12 stages plus an Endless mode — 13 in total. Five swing patterns (linear, pendulum, wave, drift, combo) with randomized amplitude and speed every drop. Later stages add wind and stronger gravity, and 12 part shapes appear, including cylinders, hexagonal and triangular prisms, L-brackets and balls. Clearing a stage unlocks the next one.

### Save Data
Language, sound setting, stars per stage, best scores and the Endless mode best height are stored in browser localStorage under the key swingstack_save_v1. To erase them, clear this site's data (site settings / storage) in your browser settings.

### Tech Notes
- Three.js 0.160 (rendering) and cannon-es 0.20 (physics) loaded as ES modules from CDN
- All SFX and BGM are procedurally generated with the WebAudio API (no audio files)
- Single-file game with no external assets

---

## 中文

### 简介
从每次摆动方式都不同的起重机上，把握时机点击屏幕放下各种形状的零件，比拼能把塔堆多高、多稳。支持电脑和智能手机，采用竖屏（9:16）布局的 3D 时机动作平衡游戏。

### 运行方法
1. 用浏览器（推荐最新版 Chrome / Edge / Safari）打开 index.html。
2. Three.js 和 cannon-es 从 CDN（jsDelivr）加载，需要联网。
3. 手机玩家可将 index.html 复制到设备上，用移动浏览器打开即可竖屏游玩。

### 玩法
- 点击屏幕（电脑端也可按空格键 / 回车键）释放起重机吊着的零件。
- 把零件堆叠到平台上的塔里，达到关卡指定高度即可过关。
- 落点严重偏离塔的中心轴或直接落到地面计为失误，3 次失误则挑战失败。
- 落点在塔中心轴 0.3 米以内可获得 PERFECT!! 奖励分。
- 过关时剩余生命数即为星级评价，分数和塔的高度会按关卡保存。

### 操作
- 点击 / 空格 / 回车：放下零件
- P 键 / Esc 键：暂停（返回菜单）
- 标题画面：语言切换（日本語 / English / 中文）、音效 开 / 关

### 关卡
共 13 种：主线关卡 1〜12 加无尽模式。摆动模式共 5 种（线性、钟摆、波动、漂移、复合），每次投放的振幅和速度都会随机变化。后段关卡有强风和更强的重力，零件共 12 种，包括圆柱、六棱柱、三棱柱、L 形支架和球体等。通过关卡后解锁下一关。

### 存档
语言、音效设置、各关星级、最佳分数和无尽模式最高高度保存在浏览器的 localStorage（键名 swingstack_save_v1）中。如需删除，请在浏览器设置中清除本站点数据（网站设置 / 存储）。

### 技术说明
- Three.js 0.160（渲染）与 cannon-es 0.20（物理）以 ES 模块方式从 CDN 加载
- 音效与 BGM 由 WebAudio API 程序化生成（无外部音频文件）
- 无需外部素材的单文件游戏
