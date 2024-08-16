## Project Title: Predicting Movie Ratings・映画の評価予測
This analysis attempts to answer the question of what the key factors are in making a good film. We analyze movie rating data using machine learning techniques to identify key factors. The most interesting results were that Running Time (the movie's length), budget, and release year were important factors that led to high rating scores. These factors may reveal reviewers' interesting biases and indicate to producers the factors making a film.

この分析は、良い映画を作るための主要な要素は何かという質問に答えることを目的としています。機械学習技術を用いて映画の評価データを分析し、主要な要素を特定しました。最も興味深い結果は、上映時間、予算、および公開年が高評価をもたらす重要な要素であることが判明したことです。これらの要素は、レビュアーの興味深いバイアスを明らかにし、プロデューサーに映画を成功させる要因を示唆しています。

## Files
**"FinalMLProject_CompleteCodes.ipynb"** This is the Python script that performs the data analysis・データ分析のパイソンスクリプト

**"Movie project  document.pdf"** This report presents the results and findings from the analysis conducted in "FinalMLProject_CompleteCodes.ipynb"・データ分析の結果

## Data set
The data set was taken from the following link・データセットはこちらのリンクから取得: https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset.

These files contain metadata for all 45,000 movies in the Full MovieLens Dataset. The dataset consists of movies released on or before July 2017. Data points include cast, crew, plot keywords, budget, revenue, posters, release dates, languages, production companies, countries, TMDB vote counts, and vote averages.

This dataset also contains 26 million ratings from 270,000 users for all 45,000 movies. Ratings are on a scale of 1-5, obtained from the official GroupLens website.


これらのファイルには、Full MovieLens データセットに含まれる45,000本の映画のメタデータが含まれています。データセットは2017年7月以前に公開された映画で構成されています。データポイントには、キャスト、クルー、プロットキーワード、予算、収益、ポスター、公開日、言語、制作会社、国、TMDBの投票数および投票平均が含まれます。

このデータセットには、270,000人のユーザーによる45,000本の映画に対する2,600万件の評価も含まれています。評価は1から5のスケールで、公式のGroupLensウェブサイトから取得されました。

## Summary of the analysis・データ分析のまとめ

**⓵ Data Loading・データ読み込み** 

**⓶ Data cleaning・データクレンジング**

**⓷ Exploratory Data Analysis (EDA)・探索的データ分析:** Conducts exploratory data analysis to understand data distributions and relationships.

データの分布や関係性を理解するために、探索的データ分析を実施。

**⓸Modeling・モデリング:** Applies machine learning models to identify patterns and make predictions.

データからパターンを特定し、予測を行うために機械学習モデルを適用。

## Results・結果

### Model Performance・モデルのパフォーマンス

**Random Forest Model・ランダムフォレストモデル:** The Random Forest Model was best suited with a Train Accuracy of 0.94, Train Precision of 0.942, Test Accuracy of 0.88, and Test Precision of 0.89.

ランダム フォレスト モデルは、"Train Precision" 0.94、"Train Accuracy" 0.942、"Test Accuracy" 0.88、"Test Precision" 0.89 で最適でした。

**Runtime・上映時間:** Runtime was found to be the second most significant predictor. Longer movies tend to receive higher critical ratings, aligning with Mark Hofmeyer's article that discusses the positive correlation between movie length and Rotten Tomato ratings.

実行時間は、映画の評価において二番目に重要な予測因子であることがわかりました。長い映画ほど、批評家から高い評価を受ける傾向があり、これはMark Hofmeyerの論文で述べられている、映画の長さとRotten Tomatoesの評価との正の相関関係と一致しています。



**Vote Count and Budget・投票数と予算:** As expected, vote count correlates with rating, and budget correlates with vote count.

予想通り、投票数は評価と相関し、予算は投票数と相関します。

**Release Year・公開日:** Surprisingly, it predicts rating, suggesting an increase in average movie ratings over time.

これは評価を予測し、時間の経過とともに映画の平均評価が上昇することを示唆しています。

**Genres・ジャンル:** Drama and Animation significantly affect ratings, possibly due to perceived prestige or family-friendliness.

ドラマとアニメーションは、おそらく評判や家族向けの認識により、視聴率に大きな影響を与えます。

**Belonging to a Collection・コレクションに属している:** Contrary to expectations, being part of a collection (e.g., sequels) is not a strong predictor of high ratings. This may be due to heightened viewer expectations and potential disappointment with sequels compared to their originals.

予想に反して、コレクション (続編など) の一部であることは、高評価の強力な予測因子ではありません。これは、オリジナルと比較して続編に対する視聴者の期待の高まりと潜在的な失望が原因である可能性があります。
