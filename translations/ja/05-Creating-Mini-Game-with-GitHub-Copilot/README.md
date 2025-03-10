- **対象者**: 開発者、DevOpsエンジニア、ソフトウェア開発マネージャー、テスター
- **学べること**: GitHub Copilot を活用してコードを作成し、コメントを追加する方法
- **作成するもの**: Copilot AI によってコードとコメントの提案が生成される C# ファイル
- **前提条件**: GitHub Copilot は無料で利用可能です。[GitHub Copilot](https://gh.io/copilot) にサインアップしてください。
- **所要時間**: このコースは1時間以内で完了可能です。

このモジュールを終了する頃には、以下のスキルを習得できます：

- 開発環境として GitHub Codespaces を体験する。
- C# コンソールアプリケーションで入出力ルーチンを開発する。
- GitHub Copilot をアシスタントとして活用する。

## 事前読書:

- [GitHub Copilot を活用したプロンプトエンジニアリング入門](https://learn.microsoft.com/training/modules/introduction-prompt-engineering-with-github-copilot/)
- [チャレンジプロジェクト - GitHub Copilot と C# を使ったミニゲームの構築](https://learn.microsoft.com/training/modules/challenge-project-create-mini-game-with-copilot-dotnet/)

## 必要条件

- [GitHub Copilot サービス](https://github.com/github-copilot/signup) を有効にしてください。

## 💪🏽 演習

[![GitHub Codespaces で開く](https://github.com/codespaces/badge.svg)](https://codespaces.new/microsoft/mastering-github-copilot-for-dotnet-csharp-developers?devcontainer_path=.devcontainer%2Fmini-game%2Fdevcontainer.json)

これまでに、GitHub Codespaces と GitHub Copilot の基本的な使い方を学びました。このチャレンジ演習では、GitHub Copilot を使用して C# でミニゲームを開発することを目標とします。

#### GitHub Codespace のテスト

1. **ソリューションエクスプローラー** を開き、**MiniGame** という名前のプロジェクトを見つけます。
1. `Program.cs` を開きます。

1. **実行とデバッグ** オプション、または Program.cs ファイル右上の再生ボタンを使ってアプリケーションを実行します。結果が次のようなコンソールメッセージに似ているか確認してください：

   ```bash
   Hello, World!
   ```
   
### ゲームロジックの作成

GitHub Copilot を使用して Codespaces が動作していることを確認したら、次は以下の仕様に基づいて GitHub Copilot の助けを借りながら C# ミニゲームのロジックを開発します：

ゲームの勝者は以下の3つの簡単なルールで決定されます：

- **グー** はチョキに勝つ。
- **チョキ** はパーに勝つ。
- **パー** はグーに勝つ。

#### ゲームのインタラクションに関する考慮事項

コンピューターが対戦相手となり、**グー**、**チョキ**、**パー** のいずれかをランダムに選択します。ゲームの操作はコンソール（ターミナル）を通じて行います。

- プレイヤーはグー、チョキ、パーのいずれかを選択でき、無効な選択をした場合は警告されます。
- 各ラウンドで、プレイヤーはリスト内のオプションを1つ入力し、対戦相手に勝ったか負けたか、または引き分けたかを通知されます。
- 各ラウンドの終わりに、プレイヤーは再度プレイするかどうかを選択できます。
- ゲーム終了時にプレイヤーのスコアを表示します。
- ミニゲームはユーザー入力を処理し、小文字に変換して、無効なオプションが入力された場合に通知します。

GitHub Codespaces 上で、GitHub Copilot がミニゲーム構築を支援できるように、適切なプロンプトを設定してください。GitHub Copilot はコメントを利用してコンテキストを把握し、作業中に役立つ提案を行います。

#### 作業の確認

1. *dotnet run* コマンドでミニゲームをコンソール上で実行します。
2. プロンプトで、*グー*、*チョキ*、*パー* のいずれかを入力します。
3. ミニゲームが、プレイヤーが勝ったか負けたか、または引き分けたかを通知することを確認します。
4. 続けてプレイすることを選択します。
5. プロンプトで *screen* と入力します。
6. ミニゲームが、プレイヤーが入力したオプションが無効であることを通知することを確認します。
7. 手順2と4を繰り返して数ラウンドプレイし、続けないことを選択します。
8. ミニゲームが終了し、スコアを表示して勝利数とラウンド数を通知することを確認します。

このチャレンジ演習を完了おめでとうございます！GitHub Copilot を使用して C# コンソールミニゲームを作成しました。

**免責事項**:  
この文書は、機械翻訳AIサービスを使用して翻訳されています。正確性を追求しておりますが、自動翻訳にはエラーや不正確な表現が含まれる可能性があることをご了承ください。原文（元の言語で書かれた文書）が信頼できる情報源とみなされるべきです。重要な情報については、専門の人間による翻訳を推奨します。本翻訳の使用に起因する誤解や誤認について、当社は一切の責任を負いません。