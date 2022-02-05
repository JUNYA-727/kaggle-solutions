## kaggle,SIGNATEで学んだ解法を学習する

- study_resnet.ipynb
  - ResNet,EfficientB0-B7の転移学習について

- Autoencoder.ipynb
  - AutoEncoderをTensorflowにて実装
  - 異常検知に対して実践　
  
  左が実際の画像､右が学習したAutoEncoderによって生成された画像(正常データ)
  ![img](https://user-images.githubusercontent.com/61785070/152639951-673f9834-2e4f-48b5-a5e4-26bac7e83975.png)
  
  
  
  異常データに対して､生成を行うと..
  
  
  ![0](https://user-images.githubusercontent.com/61785070/152640084-5ca6eceb-a03b-4309-8c6f-f060af8d7750.png)
  ![1g](https://user-images.githubusercontent.com/61785070/152640175-774a2e2e-27be-4f62-967c-93fc0b18378c.png)  

  ![3](https://user-images.githubusercontent.com/61785070/152640121-407c30ca-b955-4b92-8746-72c1c7c8d7a5.png)
  ![3g](https://user-images.githubusercontent.com/61785070/152640194-783a5278-4586-4427-8637-8a98ee19e92d.png)    

  上記のようにして画像をヒストグラムにおき､学習したAutoEncoderによって生成された画像と異常値の画像の外れ値や値が極端にずれていた場合は'異常'とみなす事ができる｡
また､コンペであり得る､アノテーションが間違っている場合やラベル付けの際に役立つ｡
