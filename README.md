# 1.概要
本リポジトリはrecursion( https://recursionist.io/ )のコンテンツである、プログラミングパラダイム・OOP内にある「Least Recently Used Cache」の成果物である。

# 2.ソースコードの説明
キャッシュへの、読み取りを O(1)、挿入を O(1)、空間計算量を O(n) で行うために、双方向リストをデータ構造として用いる。  
しかし、双方向リストの問題点として、ノードXにアクセスするために O(n) の時間を要するので、 O(1)で各ノードへとアクセスすることを可能にするハッシュマップを用いて、実装する。  
また、データの型を汎用化させるために、ジェネリクスを使っている。　