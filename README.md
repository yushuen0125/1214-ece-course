# 11/01 技術部部聚

先把教材放上來

* [投影片](https://docs.google.com/presentation/d/1YlehUyertsoipIf7xcM4AnQWa1-AVB-vFcNSBDI4cVM/edit?usp=sharing)

* [完成的 GitHub Repository](https://github.com/jerry871002/1101-ece-course)

今天教的內容有下面四個

## 終端機

### 常用的終端機指令

Windows	| MacOS / Linux |說明
:------:|:-------------:|----------
cd		|cd	            |切換目錄
cd		|pwd			|取得目前所在的位置
dir		|ls				|列出目前的檔案列表
mkdir	|mkdir			|建立新的目錄
無		|touch		    |建立檔案
copy	|cp				|複製檔案
move	|mv				|移動檔案
del		|rm				|刪除檔案
cls		|clear			|清除畫面上的內容

## Git

![git logo](https://miro.medium.com/max/380/1*OvMsmQs0Rzs_ScuiTsuWjw.png)

[Home Page](https://git-scm.com/)

### 從維基百科貼下來的內容（注意粗體跟斜體的地方）

*git*是一個***分散式版本控制軟體***，最初由**林納斯·托瓦茲**創作，於2005年以GPL釋出。最初目的是為更好地管理Linux核心開發而設計。應注意的是，這與GNU Interactive Tools（一個類似Norton Commander介面的檔案管理器）有所不同。

git最初的開發動力來自於BitKeeper和Monotone。git最初只是作為一個可以被其他前端（比如Cogito或Stgit）包裝的後端而開發的，但後來git核心已經成熟到可以獨立地用作版本控制。很多著名的軟體都使用git進行版本控制，其中包括Linux核心、X.Org伺服器和OLPC核心等專案的開發流程。

### 指令
* `git init`：初始化一個目錄，讓 Git 開始對這個目錄進行版本控制
* `git status`：查詢現在這個目錄的「狀態」
* `git add`：把更改的檔案加到暫存區
* `git commit`：讓更改的內容永久的存下來
* `git push`：把更新的內容上傳到 GitHub
* `git pull`：把  GitHub 上的東西拉回來更新
* `git clone`：可以把 GitHub 上面的 project 複製一份下來


## GitHub

![github logo](https://i.pinimg.com/originals/2c/b6/70/2cb670b6ddd8922a1c1b2fee4f6f758c.jpg)

[Home Page](https://github.com/)

[My Account](https://github.com/jerry871002)

## Markdown

![markdown logo](https://cdn.guidingtech.com/media/assets/WordPress-Import/2014/01/markdown-logo2-300x201.png)

[Home Page](https://markdown.tw/)

## 貼一段你最近寫的程式吧

我就貼上次技術部上課的內容好了

```c
int ledPin = 3;
int potPin = A0;

void setup() {
  // setup pin modes
  pinMode(ledPin, OUTPUT);
  pinMode(potPin, INPUT);
}

void loop() {
  // read the value of the pot and store it as potValue
  int potValue = analogRead(potPin);

  // turn led on and wait for the time equal to potValue
  digitalWrite(ledPin, HIGH);
  delay(potValue);

  // re-read the value of the pot and store it as potValue
  potValue = analogRead(potPin);

  // turn led off and wait for the time equal to potValue
  digitalWrite(ledPin, LOW);
  delay(potValue);
}
```
