---
author: common-member
pubDatetime: 2026-05-19T00:00:00.000Z
title: policy_scopeとdiscard gemについて
tags:
  - Rails
  - Pundit
description:
---

## やったこと
- policy_scopeの使い方を勉強
- discardについて調査


## 学んだこと
- Punditを個人開発で使用していたが、せいぜいアクション名で認可を制御した程度
- 実務では、policy_socpeでそのリソースでアクセスしてよいレコードの範囲などを制限するresolve()のほうがとてもよく使用する

- discardについて調査。
- 端的に、論理削除をするためのもの
- 情報の保持義務がある業界だと基本的に論理削除にすると思う。
- discarded_atに値が入っていれば、keptではなくなる。
- include discardだと、default_scopeでkeptを明示的に記述するのが、デフォなのかな？
