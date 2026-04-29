---
title: "【プレビュー用】新UIコンポーネント検証ページ"
date: "2026-04-21"
draft: true
description: "agent-card / cta-block / box shortcode の表示確認用ページ"
categories:
  - test
---

# 新UIコンポーネント検証ページ

このページは Phase 1 で追加した shortcode の表示崩れ・レスポンシブ挙動を確認するための**下書き**です。本番公開はしません。

## 1. 転職エージェント比較カード（agent-card）

4社横並びの比較カード。モバイルでは自動的に縦並びになります。

<div class="agent-card-grid">

{{< agent-card name="リクルートエージェント" short="RA" rating="4.8" badge="編集部イチオシ"
    tag="求人数No.1" jobs="約60万件"
    url="https://example.com/recruit"
    points="非公開求人が全体の約80%|各業界に精通した専任アドバイザー|全国47都道府県・海外対応"
    body="転職初心者〜経験者まで幅広くおすすめ。求人数の多さで選ぶならここ一択。" >}}

{{< agent-card name="doda（デューダ）" short="do" rating="4.6"
    tag="スカウト機能◎" jobs="約25万件"
    url="https://doda.jp/"
    points="スカウトメール数が業界最多水準|エージェントサービス＋求人サイトの両機能|年収査定などの診断ツールが充実"
    body="自分で探しつつ、エージェントにも相談したい人に最適。" >}}

{{< agent-card name="マイナビエージェント" short="MA" rating="4.4"
    tag="20代に強い" jobs="約6万件"
    url="https://mynavi-agent.jp/"
    points="20〜30代の若手転職に特化|中小優良企業の求人多数|書類添削・面接対策が丁寧"
    body="はじめての転職で手厚いサポートを受けたい人向け。" >}}

{{< agent-card name="type転職エージェント" short="ty" rating="4.2"
    tag="関東×IT系" jobs="約2万件"
    url="https://example.com/type"
    points="関東エリア×IT・営業職に強い|年収交渉力に定評|30代のキャリアアップ支援実績"
    body="首都圏で年収アップを狙う30代におすすめ。" >}}

</div>

---

## 2. カラーボックス（box）

既存の `box` shortcode。7色対応。

{{< box color="green" title="ポイント" >}}
転職エージェントは**複数登録が基本**です。2〜3社同時に使うことで、求人の幅・比較軸・担当者の質を見極められます。
{{< /box >}}

{{< box color="yellow" title="注意" >}}
登録後に連絡が来ないまま放置すると、求人紹介が止まることがあります。面談後は**2週間に1度**は状況共有の連絡を入れましょう。
{{< /box >}}

{{< box color="cyan" title="ヒント" >}}
担当者と合わないと感じたら、**担当変更依頼**を遠慮なく伝えてOK。エージェント側も想定内の対応なので関係が悪くなることはありません。
{{< /box >}}

{{< box color="cream" title="まとめ" >}}
自分に合うエージェントは「求人の質 × 担当者との相性」で決まります。まずは大手2社＋特化型1社の**3社登録**から始めるのが王道です。
{{< /box >}}

---

## 3. 記事末尾CTA（cta-block フル版）

メインボタン＋サブボタン＋信頼バッジ付き。

{{< cta-block
    title="気になったエージェントに、今すぐ無料登録"
    sub="登録は5分・完全無料・あなたのキャリアを一歩前へ"
    main-label="リクルートエージェントに無料登録"
    main-url="https://example.com/recruit"
    sub-label="dodaで求人を見る"
    sub-url="https://doda.jp/"
    badges="完全無料|登録5分|非公開求人あり|24時間対応" >}}
迷ったらまずは**大手2社**に登録してみるのがおすすめ。合わなければ退会も簡単です。
{{< /cta-block >}}

---

## 4. CTA コンパクト版

記事の途中に差し込む用の軽量版。

{{< cta-block compact="true"
    title="まずは1社だけ無料相談してみる"
    sub="所要時間5分、登録後すぐ面談予約が可能です"
    main-label="無料で相談する"
    main-url="https://example.com/recruit" >}}{{< /cta-block >}}

---

以上、Phase 1 で追加した3コンポーネント（agent-card / cta-block / box）の検証ページでした。
