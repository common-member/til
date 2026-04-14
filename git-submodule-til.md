---
author: common-member
pubDatetime: 2026-04-15T00:00:00.000Z
title: Git Submoduleで別リポジトリのコンテンツをブログに組み込む
tags:
  - git
  - github-actions
description: TIL記事を別リポジトリで管理し、Git Submoduleでブログに組み込む構成を構築した。
---

## やったこと

TIL記事を専用リポジトリ（`common-member/til`）で管理し、ブログ（`common-member.github.io`）にGit Submoduleとして組み込む構成を作った。

## 学んだこと

- `git submodule add <url> <path>` でサブモジュールを追加できる
- GitHub Actionsでサブモジュールを使うには、`actions/checkout@v4`の`submodules: true`が必要
- `git submodule update --remote`で最新のコミットを取得できる
- 別リポジトリからデプロイをトリガーするには`repository_dispatch`とPATが必要
