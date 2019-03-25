---
description: 所謂：工欲善其事，必先利其器，如果ADB本來就出現問題，後面的介紹當然不用玩。
---

# 第一節：檢查ADB工具運作\(Windows系統環境\)

　　既然是使用Android Studio IDE工具開發，當然是需要下載Android Studio，不過這邊就先不多介紹。  
相信會來看這篇文章，都已經學會基本的Android Studio安裝及使用方法吧。  
不過還是給個下載連結好了：[https://developer.android.com/studio](https://developer.android.com/studio)

　　執行Android Studio並開啟專案後，下方有一個叫Terminal的工具，將它顯示出來。

![Terminal&#x4F4D;&#x7F6E;](.gitbook/assets/terminal-wei-zhi.png)

　　Terminal畫面相信大家都不會陌生，就是熟悉Windows的cmd指令視窗。

　　接下來就是介紹本篇主角ADB \(Android Debug Bridge\)這個工具，有在開發Android App相信對這名字不會陌生，在Windows版本的Android Studio如果是使用預設安裝的話，ADB的路徑一般會放在：

```text
C:\Users\ <UserName> \AppData\Local\Android\Sdk\platform-tools
```

![&#x8DEF;&#x5F91;&#x7BC4;&#x4F8B;&#x5716;](.gitbook/assets/lu-jing-fan-li-tu.png)

　　在路徑中的AppData必須要顯示隱藏檔案才會看到，在platform-tools資料夾裡面，會有一個叫adb.exe的檔案，就是我們必須要用到的工具。下一步請你把adb的路徑複製下來。回到Android Studio的Terminal畫面使用cd指令再貼上你的路徑後按Enter。

```text
cd C:\Users\ <UserName> \AppData\Local\Android\Sdk\platform-tools
```

![&#x8B8A;&#x66F4;&#x7576;&#x524D;&#x76EE;&#x9304;&#x7BC4;&#x4F8B;](.gitbook/assets/bian-geng-dang-qian-mu-lu-fan-li.png)

路徑變更後可以輸入：

```text
adb version
```

![&#x6AA2;&#x67E5;ADB&#x6307;&#x4EE4;](.gitbook/assets/jian-cha-adb-zhi-ling.png)

　　如果成功顯示ADB的版本，代表你的ADB工具是可以正常運作的，下一步將帶領如何使用ADB指令進行對裝置TCP/IP傳輸設定。







{% code-tabs %}
{% code-tabs-item title="第一節懶人包指令：" %}
```text
//首先取得ADB的路徑，<UserName>是你Windows使用者名稱
cd C:\Users\ <UserName> \AppData\Local\Android\Sdk\platform-tools

//檢查ADB相關指令是否能夠執行
adb version
```
{% endcode-tabs-item %}
{% endcode-tabs %}

