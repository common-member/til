---
author: common-member
pubDatetime: 2026-04-13T00:00:00.000Z
title: AstroPaperでTILブログを構築した
tags:
  - astro
  - github-pages
description: AstroPaperテーマを使ってGitHub Pages上にTILブログを構築した際の学び。
---

## やったこと

AstroPaperテーマを使って、GitHub Pages上にTILブログを構築した。

## 学んだこと

- AstroPaperはAstro v5ベースのブログテーマで、SEO対応やダークモードが標準搭載されている
- GitHub Pagesのデプロイには、Settings > Pages > SourceをGitHub Actionsに変更する必要がある
- `withastro/action@v3`を使う場合、`package.json`に`packageManager`フィールドが必要
