## 埋め込み空間分析のためのユークリッド距離を用いた拡散モデルのガイダンス

<!--
**1116211089-MikiYanobu/1116211089-MikiYanobu** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

### 概要
近年，埋め込みモデルによって，自然言語-画像のペアの予測を高精度なゼロショット転移で行うなどの，異なるモダリティ間の高精度な検索が可能となった．
埋め込みモデルの埋め込み空間は，関連するテキストと画像のペアは近く，そうでないペアは遠くに写像されるように学習される．しかしながら，モデルが学習した埋め込み空間が，一般性のあるものなのかは分かっていない．そこで，本研究では，埋め込み空間を分析するために，任意の特徴量から画像生成を行うデコーダを作成することを目的とする．  
このデコーダを用いれば，異なる画像A，Bの2点の特徴量の間に存在する特徴量から画像生成を行い，画像Aから画像Bに徐々に遷移するのか，そうでないのかを視覚的に調べるというような分析が可能になる．  
デコーダを構築するにあたり、拡散モデルのガイダンスという手法を用いる。拡散モデルを汎用的な画像生成器として使用し，何らかの基準が満たされる画像が生成されるように誘導するガイダンス機能を持たせることで，再学習なしで，柔軟な画像生成を実現する．特に，本研究では[Bansalらのuniveisal guidance](https://github.com/arpitbansal297/Universal-Guided-Diffusion)に変更を加え，目的の特徴量と現時点での生成画像の特徴量とのユークリッド距離が小さくなるようなガイダンスを提案する．
### 実行環境
### 各フォルダの説明
### 実行方法
### 参考文献
```
@misc{bansal2023universalguidancediffusionmodels,
      title={Universal Guidance for Diffusion Models}, 
      author={Arpit Bansal and Hong-Min Chu and Avi Schwarzschild and Soumyadip Sengupta and Micah Goldblum and Jonas Geiping and Tom Goldstein},
      year={2023},
      eprint={2302.07121},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2302.07121}, 
}
```
