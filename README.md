# Algorithm_Ai
AI uchun kerak boladigan Algorithmlarni pythonda yozilishi. Writing algorithms needed for AI in Python. AIに必要なアルゴリズムをPythonで記述します。

Hozir KNN va KMeans algorithmlari bor ular haqida:
KNN - bu yangi ma'lumot  yoki dataga eng yaqin turgan K ta qo'shning  sinfiga qarab bu data (ma'lumot)  qaysi sinfga tegishli bo'lishini bashorat qiladi.
Matematika asosi: Masofani hisoblash uchun ko'pincha Evklid masofasi yoki inglizcha (Euclidean distance) dan foydalaniladi.
KMeans- ma'lumotlarni o'xshashligi bo'yicha K ta klasterga ajratuvchi Unsupervised learning algorithmi.
Algorithmni ishlashi:
 1. Algorithmi tasodifiy nuqta tanlaydi va u markaz bo'ladi.
 2. Har bir nuqtani eng yaqin markazlarga biriktiradi.
 3. Markazlarni yangilaydi va eng ideal markaz topilsa to'xtaydi.
Optimal Kta sinfni ajratishda  'Elbow Method' (Tirsak usuli)  orqali foydalaniladi .

KNN is a Supervised Learning algorithm used for classification. It predicts the class of a new data point based on the classes of its $K$ nearest neighbors.
How it works : When a new data point is introduced, the algorithm identifies the $K$ closest points in the training dataset. The new point is then assigned to the most frequent class among those neighbors.
Mathematical Foundation:
To calculate the proximity between points, Euclidean Distance is most commonly used
K-Means is an Unsupervised Learning algorithm that groups data into $K$ distinct clusters based on their similarities.
Algorithm Workflow:
    1. Centroid Initialization: The algorithm randomly selects K points to act as initial cluster centers (centroids).
    2. Assignment: Each data point is assigned to the nearest centroid.
    3. Update: Centroids are recalculated by taking the average (mean) of all points assigned to that cluster.
    4. Convergence: This process repeats until the centroids stabilize (the "ideal" centers are found).
The 'Elbow Method' is used to determine the optimal number of clusters K. It involves plotting the within-cluster sum of squares (WCSS) and finding the "elbow" point where the rate of decrease significantly slows down.
🛠 Tech Stack
Python
NumPy (Numerical computations)
Matplotlib (Visualizing results)
Pandas

機械学習アルゴリズム: KNN & K-Means

このリポジトリには、機械学習の基本となる2つのアルゴリズム（K近傍法: KNN と K-Means法）の実装が含まれています。

1. K近傍法 (K-Nearest Neighbors: KNN)

KNNは、分類に使用される 教師あり学習 (Supervised Learning) アルゴリズムです。新しいデータポイントのクラスを、その近くにある K 個の隣接データのクラスに基づいて予測します。

アルゴリズムの仕組み:
新しいデータが導入されると、アルゴリズムは学習データセットの中から最も近い K 個の点を選び出します。その後、それらの隣接データの中で最も多いクラスを新しいデータのクラスとして割り当てます。

数学的基礎:
点と点の間の距離を計算するために、一般的に ユークリッド距離 (Euclidean Distance) が使用されます。

2. K-Means法 (K-Means Clustering)

K-Meansは、データの類似性に基づいてデータを K 個の異なるクラスタにグループ化する 教師なし学習 (Unsupervised Learning) アルゴリズムです。

アルゴリズムのワークフロー:
1. セントロイドの初期化: アルゴリズムは、初期のクラスタ中心（セントロイド）として K 個の点をランダムに選択します。
2. 割り当て: 各データポイントを最も近いセントロイドに割り当てます。
3. 更新: 各クラスタに割り当てられたすべての点の平均値を計算し、セントロイドを再配置します。
4. 収束: セントロイドが安定する（理想的な中心が見つかる）まで、このプロセスを繰り返します。

最適なK値の決定:
クラスタ数 K を決定するために エルボー法 (Elbow Method) が使用されます。これは、クラスタ内誤差平方和 (WCSS) をプロットし、減少率が著しく低下する「エルボー（肘）」の点を見つける手法です。

技術スタック (Tech Stack)
Python
NumPy (数値計算)
Matplotlib (結果の可視化)
Pandas