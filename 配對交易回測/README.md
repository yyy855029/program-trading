# 配對交易回測
## 作品:
### 玉晶光/亞光Z-Score配對交易策略
## 步驟:
### 挑選配對交易個股對象:
* 以光學股為對象從Yahoo Finance抓取股價資料
* 計算光學股個股間調整後收盤價、變動比率相關係數
* 選擇調整後收盤價變動比率最高的玉晶光、亞光作為配對交易對象
### 計算Z-Score:
* 計算玉晶光/亞光調整後收盤價之價格比率
* 以價格比率的長短天期MA和標準差計算Z-Score
### 根據Z-Score收斂策略建立多空部位:
* 若當期Z-Score由下往上穿過1  : 則下期放空玉晶光、做多亞光
* 若當期Z-Score由上往下穿過-1 : 則下期放空亞光、做多玉晶光
### 績效呈現和最佳化參數:
* 在樣本內資料最佳化根據報酬選擇長短天期MA參數
* 在全樣本資料檢驗績效報酬 
## 示意圖:
### 挑選配對交易個股對象:
![picture1](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E8%AA%BF%E6%95%B4%E5%BE%8C%E6%94%B6%E7%9B%A4%E5%83%B9%E7%9B%B8%E9%97%9C%E4%BF%82%E6%95%B8%E7%86%B1%E5%BA%A6%E5%9C%96.png)
![picture2](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E8%AA%BF%E6%95%B4%E5%BE%8C%E6%94%B6%E7%9B%A4%E5%83%B9%E8%AE%8A%E5%8C%96%E7%8E%87%E7%9B%B8%E9%97%9C%E4%BF%82%E6%95%B8%E7%86%B1%E5%BA%A6%E5%9C%96.png)  

![picture3](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E8%AA%BF%E6%95%B4%E5%BE%8C%E6%94%B6%E7%9B%A4%E5%83%B9.png)
### 計算Z-Score:
![picture4](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E5%83%B9%E6%A0%BC%E6%AF%94%E7%8E%87.png)
![picture5](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/z_score.png)
### 根據Z-Score收斂策略建立多空部位:
![picture6](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E8%A8%8A%E8%99%9F%E5%92%8C%E9%83%A8%E4%BD%8D%E5%9C%96.png)
### 績效呈現和最佳化參數:
![picture7](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E7%B4%AF%E7%A9%8D%E5%A0%B1%E9%85%AC%E5%92%8C%E7%B4%AF%E7%A9%8D%E6%9C%80%E5%A4%A7%E5%A0%B1%E9%85%AC.png)
![picture8](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E5%80%8B%E8%82%A1%E5%A0%B1%E9%85%AC%E5%92%8C%E7%B8%BD%E5%A0%B1%E9%85%AC.png)
![picture9](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E5%B9%B3%E5%80%89%E6%AC%8A%E7%9B%8A%E6%9B%B2%E7%B7%9A%E5%92%8C%E7%B8%BE%E6%95%88%E6%8B%89%E5%9B%9E.png)
![picture10](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E6%AF%8F%E6%9C%88%E7%8D%B2%E5%88%A9%E5%92%8C%E8%99%A7%E6%90%8D.png)
![picture11](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E6%AF%8F%E6%9C%88%E7%8D%B2%E5%88%A9%E5%92%8C%E8%99%A7%E6%90%8D.png)
![picture12](https://github.com/yyy855029/program_trading_practice/blob/master/%E9%85%8D%E5%B0%8D%E4%BA%A4%E6%98%93%E5%9B%9E%E6%B8%AC/Img/%E6%9C%80%E4%BD%B3%E5%8C%963D%E5%9C%96.png)
## 使用程式:
Python

