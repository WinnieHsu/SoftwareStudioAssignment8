# SoftwareStudioAssignment8

這份作業主要是練習將手機上的計算機App連結到電腦開的Server，
並將計算結果從手機Client端傳到Server端

在Server.java主要就是新增JFrame和JLabel，將Client端傳進的String s顯示在JFrame上

而在Client端的MainActivity.java主要是將連線後的頁面改成計算機的畫面(calculator_main.xml)
並將上次Lab10計算機的code給加進來，計算後將結果印到結果頁(result_page.xml)
而回傳計算結果回Server則是透過 OutputStream out = socket.getOutputStream();

這次作業遇到最大的困難是我在編寫MainActivity的時候忘記新增和開始thread了，
所以計算出的結果一直無法回傳給Server...
經過這次慘痛經驗我明白到新增thread的重要性!!!!!!!!!!
