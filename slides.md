---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shiki
lineNumbers: True
drawings:
  persist: false
css: unocss
title: Medical Device Presentation by G1
transition: slide-left
---

# Medical Devices
# Display & Healthcare

Group 1 Presents 

<div class="pt-12">
  <span class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    Meet the Team <carbon:arrow-right class="inline"/>
  </span>
</div> 

<font class="absolute bottom-5 right-5"><SlideCurrentNo />/<SlidesTotal /></font>
---
transition: slide-up
preload: false
---

# Meet the Team

<br>
<div grid="~ cols-5 gap-12" >


  <div>
    <img 
      v-motion
      :initial="{x: 300, y: -100, scale: 1.2, rotate: -50}"
      :enter="{x:-130, y:-63, scale:0.273, rotate:0, transition: {delay:500,duration:1000}}"
      class="absolute top-0 left-0 right-0 bottom-0"
      src="m1.jpg"> <br> 
    <div    
      class="text-5xl absolute text-[#2B90B6] -z-1"
      align="center"
      v-motion
      :initial="{ x: -40, opacity: 0}"
      :enter="{ x: 0, y:140, opacity: 1, transition: { delay: 2000, duration: 1000 } }">
      卓寧文 <br>
      電機博 <br>
  </div>
  </div>

  <div v-after>
    <img src="hcw.jpg"> <br>
    <div
      class="text-5xl absolute text-[#2B90B6] -z-1"
      align="center"
      v-motion
      :initial="{ x: -40, opacity: 0}"
      :enter="{ x: 0, opacity: 1, transition: { delay: 3000, duration: 1000 } }">
      邱浩宸 <br> 
      電信碩 <br>
    </div>
  </div>

  <div v-after>
  <img src="m2.png"> <br>
    <div
      class="text-5xl absolute text-[#2B90B6] -z-1"
      align="center"
      v-motion
      :initial="{ x: -40, opacity: 0}"
      :enter="{ x: 0, opacity: 1, transition: { delay: 3000, duration: 1000 } }">
      何柏翰 <br> 
      電信碩 <br>
    </div>
  </div>

  <div v-after>
  <img src="g1.png"> <br>
   <div
      class="text-5xl absolute text-[#2B90B6] -z-1"
      align="center"
      v-motion
      :initial="{ x: -40, opacity: 0}"
      :enter="{ x: 0, opacity: 1, transition: { delay: 3000, duration: 1000 } }">
      劉宜萱 <br> 
      生傳二 <br>  
    </div>
  </div>

  <div v-after>
  <img src="g2.jpg"> <br>
    <div    
      class="text-5xl absolute text-[#2B90B6] -z-1"
      align="center"
      v-motion
      :initial="{ x: -40, opacity: 0}"
      :enter="{ x: 0, opacity: 1, transition: { delay: 3000, duration: 1000 } }">
      陳姿妤 <br> 
      外文四 <br>
    </div>
  </div>

</div>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<font class="absolute bottom-5 right-5"><SlideCurrentNo />/<SlidesTotal /></font>

---
layout: default
transition: fade-out
---

# Table of contents

<Toc></Toc>

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<font class="absolute bottom-5 right-5"><SlideCurrentNo />/<SlidesTotal /></font>

---
layout: two-cols
transition: fade-out
---

# 醫療產業趨勢: 精準醫學

<div v-click>

* 精準 = Personalized Medicare + Healthcare
  * 個人化醫療: 專注在較微觀"個人化"
  * 健康照護(Healthcare): 專注在較宏觀的醫療量能
</div>

<div v-click>

* 目的在於針對各個病例做最有效的
  1. **預測&預防** 
  2. **精準診斷** 
  3. **最佳治療效果**
</div>

<div v-click>

* 實際的多領域新穎方法:
  1. 基因檢測/定序
  2. 影像醫學
  3. AI&巨量資料
  4. 醫用電子器材
  5. etc...
</div>

::right::
<br><br>

```mermaid
flowchart TB
  1A(個人化醫療) --aggregate--> A(((精準醫療)))
  2A(健康照護) --aggregate--> A
  A --> B(預測預防)
  A --> C(精準診斷)
  A --> D(治療方案)
  
  subgraph tool
  T1(基因定序) -.- T2(影像醫學)
  T2 -.- T3(醫用電子)
  T3 -.- T4(AI, 巨量資料)
  end
  B -.-> tool
  C -.-> tool
  D -.-> tool
```

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<font class="absolute bottom-0 right-0"><SlideCurrentNo />/<SlidesTotal /></font>

---
transition: fade-out
---

# 跨領域工具實例

### 1. Motif Search: 基因定序$\times$巨量資料
### 2. Medical Display: 影像醫學$\times$醫用電子
### 3. U-net: 影像醫學$\times$AI
### 4. etc ..<br>

<img src="trend.png" width=400 class="absolute left-10 bottom-10">

<font class="absolute top-61 right-19" size=4>台灣既有的硬體優勢結合影像醫學產業趨勢<br>-> <strong>Medical Display </strong></font>
<arrow x1="570" y1="230" x2="490" y2="150" color="#564" width="2" arrowSize="1"/>
<arrow x1="550" y1="303" x2="250" y2="430" color="#564" width="2" arrowSize="1"/>

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<font class="absolute bottom-5 right-5"><SlideCurrentNo />/<SlidesTotal /></font>

---
transition: slide-up
level: 2
---
# Medical Display 介紹

* 醫用顯示器所需可靠度要求極高:
  * 任何醫學圖像在顯示器的黑點/變形/色差不能是因顯示器本身造成
  * 對任何影像傳輸的延遲幾乎零容忍 (光纖傳輸)
<div v-click>

* 重大實際應用場景
  * **遠距手術** e.g. 達文西手臂
  * **侵入式檢測/治療** e.g. 內視鏡
</div>

<div v-click>

* 所有醫用電子實際商轉過程

```mermaid
flowchart LR
A(醫用電子儀器設計) --> B(法規及標準檢測) --> C(上市販售)
```
</div>

<div v-click>
<br>
實際商轉例子: 
</div>


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>


<font class="absolute bottom-5 right-5"><SlideCurrentNo />/<SlidesTotal /></font>

---
transition: slide-up
level: 2
layout: two-cols
---

# 實際商轉例子

* 以一包含醫規顯示器的醫療檢測系統為例
<div v-click>

* **法規:** 各國依據風險或侵入程度不同分類
  * e.g. 美國 FDA 510k 將此產品歸為二級
</div>

<div v-click>

* **標準:** 獨立於法規但會嚴重影響商品市場價值

**重要醫療等級標準:**
</div>

<div v-click>

1. IEC-60601: 電磁相容及安全規範
2. ISO-14971: 操作風險管理
3. IEC-62366: 可用性工程 (usability)
4. IEC-62304: 軟韌體開發流程規範 生命週期及憑證 
5. Manangement of Cybersecurity in Medical Device: 2016
</div>


<div v-click>

**AI, 醫用物聯網, 醫療資訊系統等等受到(4), (5)的限制** 

</div>


::right::
<img src="reg.png">


<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 20%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>

<font class="absolute bottom-5 right-5"><SlideCurrentNo />/<SlidesTotal /></font>
