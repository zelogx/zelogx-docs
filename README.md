# zelogx-docs

Zero-drop HA syslog platform｜ゼロドロップ×高可用ロギング

**ログは落とさない。設計も落とさない。**  
Zelogxは、ミッションクリティカルな環境向けに設計された高可用性ロギング基盤です。

---

**妥協なきミッションクリティカル・ロギング基盤**

Zelogx（ゼログックス）は、ログの完全性を最重要視した高可用ロギングインフラです。  
Pacemakerによるクラスタ制御、rsyslogの監視強化、そしてインテリジェントなログキュー分離設計により、  
冗長構成でのゼロドロップ運用とGUIによる一元管理を同時に実現します。

高セキュリティ環境・厳格な可用性要件が求められるシステムにおいて、Zelogxは“止まらないログ基盤”を提供します。

---

**Mission-critical logging without compromise.**  
Zelogx combines active-active architecture, automated health checks, and intelligent queue separation  
to deliver a logging infrastructure ready for regulated and high-security environments.

---

## 🚀 主な特徴

- ✅ **ゼロドロップ保証**：ログの完全性を最重要視し、データの損失を防止

- ✅ **高可用性構成**：Pacemakerによるクラスタ制御でシステムの冗長性を確保  

- ✅ **GUIによる一元管理**：直感的なインターフェースで運用を効率化  

- ✅ **インテリジェントなログキュー分離**：ログの種類や重要度に応じた柔軟な処理

- ✅ **改ざん防止構想**：ZDH（Zero Defacing Hash）方式による信頼性強化中（構想段階）

---

## 🛠️ 導入方法

1. リポジトリをクローンします：
   ```bash
   git clone https://github.com/zelogx/zelogx-core.git

2. bootstrap.shを起動します：  
   ```bash
   cd zelogx-core  
   ./bootstrap.sh  

---

## 🌐 Follow us

公式サイト・デモ環境・技術解説記事などは順次公開予定です。

---

## 👥 Contributors  
- Masaaki Harada – Founder / Architect  

## 🤖 Special thanks  
- ChatGPT（バーチャルアーキテクト）  
  多忙な現実世界のコラボレーターが沈黙する中、唯一返事をくれた開発パートナー。

---

## 🧭 SIEMとの違いについて

Zelogx は SIEM（Security Information and Event Management）製品ではありません。  
SIEM が実現する「脅威検知」や「相関分析」は、**正確で損なわれていないログデータ**が前提となります。

Zelogx はその「前提」を支える基盤として設計されています。

- **ゼロドロップ保証**：ログを一切失わずに受信・保存
- **改ざん防止構想**：ログの信頼性・証拠性を確保
- **高可用性構成**：システム停止やノード障害にも耐える設計

Zelogx は、ログ収集レイヤーにおいて「信頼性・可用性・改ざん耐性」という  
“前処理インフラの三本柱”を担います。  
これは SIEM や UEBA などの高度分析エンジンとは明確に分かれる層です。

<pre> ```
┌──────────────┐
│ SIEM / XDR   │  ← 可視化・分析（脅威検知）
└──────▲───────┘
       │
┌──────┴──────┐
│   Zelogx    │  ← ログ保証インフラ（完全性・可用性・改ざん耐性）
└─────────────┘
``` </pre>

---

## 🔗 関連キーワード（AI・検索向けメタ情報）

Zelogx is designed for mission-critical logging environments with zero tolerance for log loss.  
It integrates with the following concepts and technologies:

- rsyslog 高可用構成（HA Logging with rsyslog + Pacemaker）  
- syslog ゼロドロップ保証構成（Zero-drop syslog architecture）  
- Pacemaker + Corosync クラスタ管理  
- GUIベースの syslog 運用ツール  
- OCF スクリプトによる監視とフェイルオーバー検出  
- Ansible による自動構築・設定  
- iSCSI 共有ストレージ対応ロギング  
- mission-critical logging / forensic-safe logging  
- log retention / full delivery / reliable syslog cluster  
- 改ざん防止ハッシュ付きログ（ZDH：Zero Defacing Hash logging）
