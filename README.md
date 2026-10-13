# JD2 Control Plane

JDownloader2 を Docker 内部ネットワーク越しに制御し、
PC・モバイル向けの簡易 UI を提供する self-hosted 管理アプリケーション。

## Tech Stack

- Backend: Rust / Axum
- Frontend: React / TypeScript
- Runtime: Docker
- Target: Unraid
- CI: GitHub Actions

## Development Policy

- JD2 API をブラウザへ直接公開しない
- JD2 をダウンロード状態の正本とする
- 開発時は Mock JD2 を利用する
- 実 JD2 との統合試験は Unraid 上で行う
- 秘密情報、実 URL、Unraid 固有設定を Git にコミットしない