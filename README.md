# Calc_Matrix_Study  


三次元ジオメトリの変換行列に関して解きたい問題がある。変換行列を使うということをあまりやったことがないのでここで試していきたい。  

Rhino for Mac では、GhPython から行列の要素にアクセスできず一日二日格闘して結局駄目府だったが、Windows を使ったら普通にできたので、Mac 版での動作は知りません。  


## アフィン変換  

アフィン変換 = 平行移動を伴う線形写像  

線形写像 = 回転（Rotation）、拡大縮小（Differential Scaling）、せん断（Skew）  


---  


## オペレーション  

### Rhino における変換行列  

ライノで変換行列が見えるのは、ブロックインスタンスを扱うときくらい？  

![rhino_blockinstance](_images/matrix_0.png)  


### Grasshopper における変換行列  

Grasshopper では、Transform 型がサポートされており、コンポーネントのカテゴリにも Transform がある。  

個人的に面白いなと思ったのは、オブジェクトを移動する Move コンポーネントや、オブジェクトを回転させる Rotate コンポーネントから、変換結果のオブジェクトと合わせて、変換行列が出力される。  

使いどころはわからないが、逆行列で戻せよという意味だろうか。  

（DisplayMatrix とかいうコンポーネントあったんですね。）  

![rhino_blockinstance](_images/matrix_1.png)  



### Grasshopper + GhPython における変換行列  




### Python3 + Numpy  




---  


## 演算  


### Python3 + Numpy の結果を Grasshopper で  


---  


## Ref  

デジタル画像と定量化その６：アフィン変換・位置合わせ  
  - [http://www2.riken.jp/brict/Yoshizawa/Lectures/Kyuusyu/Lectures2011_06.pdf](http://www2.riken.jp/brict/Yoshizawa/Lectures/Kyuusyu/Lectures2011_06.pdf)  


ゲームグラフィックス特論  
  - [https://tokoik.github.io/gg/ggbook03.pdf](https://tokoik.github.io/gg/ggbook03.pdf)  