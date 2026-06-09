# Gen Nishizumi - Portfolio Draft

## 概要（Concept）
このポートフォリオは、「作業者（コーダー）」としてのスキルアピールを一切排除し、「次世代アーキテクチャを設計・実装する**アーキテクト**」としての圧倒的な権威付けと、レガシーシステムへのアンチテーゼを示すためのものです。

---

# 🌐 サイト構成ドラフト (Webページの構造)

## 1. Hero Section (ファーストビュー)
*   **Catchcopy:** 
    *   「If文とSQLを捨てよ。多次元幾何学が導く O(1) の制約解決。」
    *   (Eng) "Discard If-statements and SQL. Achieving O(1) Constraint Resolution through Multi-dimensional Geometry."
*   **Subtext:** 
    *   膨大な計算量を強いるレガシーな探索アルゴリズムやリレーショナルデータベースの限界を突破する。AIのセマンティック空間と幾何学処理を融合させた次世代アーキテクチャ「Microforce」の設計と実装。
*   **Visual Idea:** 複雑なノードが幾何学的な図形（マスク）によって一瞬で一つの点に収束するような、プレミアムなアニメーションやダークモードベースの洗練されたUI。

## 2. Publications & Research (学術・技術発信)
*ただのエンジニアではなく、パラダイムを創出し世界に問う存在であることを証明するセクション。*

*   **[Paper] CERN Zenodo (1):** 
    *   **Title:** "Geometric Resolution Paradigm for NP-Hard Constraints" (仮称の流用、必要に応じて調整)
    *   **Description:** 既存の数理最適化ソルバーが抱える計算量爆発に対し、多次元空間の幾何学的マスク交差により解を O(1) で特定するパラダイムシフト。
    *   **Link:** `https://zenodo.org/records/20602701`
*   **[Paper] CERN Zenodo (2):** 
    *   **Description:** (論文の概要をここに記載)
    *   **Link:** `https://zenodo.org/records/20580181`
*   **[Article] Zenn / Tech Blog:**
    *   **Title:** 「If文とSQLを完全に捨てる — 次世代AI時代のデータ基盤」
    *   **Description:** 既存SQLデータベースベンダーへ向けた技術的アンチテーゼ。手続き型ロジックの廃止と、完全なデータドリブン・幾何学エンジンへの移行記録。
    *   **Link:** `https://zenn.dev/unizho/articles/b4b5cd7e53f89a`

## 3. Architectures & Deliverables (アーキテクチャと成果物)
*理論だけでなく、実際に稼働するプロダクト・エンジンを持っていることの証明。*

*   **Core Engine: Microforce**
    *   **Overview:** NP困難な制約充足問題を、多次元テンソル（幾何学）処理により瞬時に解決する独自エンジン。
    *   **Repository:** `https://github.com/2423gen-stack/microforce-core`
*   **Live Demo: Autonomous Shift Scheduler**
    *   **Overview:** Microforceエンジンを基盤に構築された実稼働シフト自動作成システム。複雑な人間関係や労働条件の制約を幾何学的に解決。
    *   **Repository:** `https://github.com/2423gen-stack/microforce-shift`
    *   **Link:** `https://shift.okyn.net`

## 4. Philosophy & Technology Stack (技術哲学と現在のツールボックス)
*「〇〇年経験があります」という労働者目線ではなく、「今の最適な道具としてこれらを選定している」という見せ方。*

*   **Statement:** 
    *   「プログラミング言語やフレームワークは、アーキテクチャを表現するための単なる道具に過ぎない。重要なのは、どのような制約を打ち破り、どのような城を築くかである。」
*   **Current Toolkit:**
    *   **Core Logic:** Python, LLM (Gemini Advanced Context)
    *   **Persistence & Ops:** PostgreSQL, Docker, Linux (Ubuntu Pro)
    *   **Frontend Representation:** Astro, Svelte, Tailwind CSS
    *   **Business Automation:** n8n + AI

## 5. Profile (西住玄 - Gen Nishizumi)
*異色の経歴から生まれる、技術とデザインの特異な融合。*

*   **Name:** 西住玄 (Gen Nishizumi)
*   **Role:** フリーランス AIアーキテクト / Paradigm Designer
*   **Background:**
    *   多摩美術大学デザイン科 卒業。
    *   東京慈恵会医科大学附属病院にてサーバー管理者として基盤運用に従事。
    *   独立後、現在はAIアーキテクトとして活動。n8n+AIを基幹としたバックオフィス業務（事務処理）の自動化ソリューションの開発・提供や、モダンなWebサービス開発を手掛ける。
    *   美大出身のデザイン思考と、医療現場におけるミッションクリティカルなサーバー運用経験が、現在の「堅牢かつ洗練されたAIアーキテクチャ」の設計思想の原点となっている。

---

## 💻 開発の段取り (Next Steps)
1.  **プロジェクト初期化:** `Astro` + `Tailwind CSS` + `Svelte` を用いて、この `/home/gen/Projects/tec-portfolio` ディレクトリに環境を構築。
2.  **デザインシステム構築:** 「アーキテクト」にふさわしい、黒と鮮やかなアクセントカラーを用いたプレミアムなUI。
3.  **コンテンツ流し込み:** 上記のドラフト文面をコンポーネントに落とし込み、パララックス効果等でリッチに魅せる。
4.  **Cloudflare Pages等へのデプロイ:** サーバーレスで爆速配信。
