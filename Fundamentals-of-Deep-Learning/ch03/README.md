# Tensorflowを用いたニューラルネットワークの構築

## Tensorflowでのセッション
```
python session.py
```

## Variableのスコープと共有
複雑なモデルを作成する場合、一度インスタンス化したVariableを共有し、再利用できるといい
Variableの有効範囲を指定する  
tf.get_variable(<name>, <shape>, <initializer>)
    指定された名前のVariableが存在するかチェック
tf.variable_scope<(scope_name)>
    名前空間を管理し、tf.get_variableの有効範囲を判断する
```
python scope2.py
```


## ロジスティク回帰モデルの実装
```
python logistic_regression.py
```

### 計算グラフと学習を可視化
```
tensorboard --logdir=</file_path>
```
