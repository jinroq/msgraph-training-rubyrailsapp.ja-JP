# <a name="contributing-to-microsoft-graph-training-repositories"></a>Microsoft のトレーニング リポジトリGraphに貢献する

このプロジェクトに貢献して下さい。 プル要求を送信する前に、次の点を考慮してください。

## <a name="overview"></a>概要

このリポジトリのコードには、次の 3 つの目的があります。

- チュートリアル フォルダー内の[](/tutorial)Markdown ファイルは、Microsoft の [チュートリアル] ページでチュートリアル[Graph発行](https://docs.microsoft.com/graph/tutorials)されます。
- デモ フォルダー内のサンプル [プロジェクト](/demo)は、Microsoft のクイック スタートGraph [ソースです](https://developer.microsoft.com/graph/quick-start)。**\***
- デモ フォルダー内のサンプル プロジェクトは、GitHubから直接ダウンロード可能で、簡単な構成の後に実行する必要があります。

> **\*** すべてのトレーニング リポジトリがクイック スタートとして使用できる (まだ) という場合はありません。

これは、ある場所での変更が別の場所で変更を必要とする可能性がある点に気を付け、物事を同期するために重要です。可能な限り、Markdown ファイルは (カスタム構文を使用して) ソース コード ファイルを直接参照し、ソース内のコードを更新すると Markdown のコードが自動的に `:::code` 更新されます。

## <a name="updating-code"></a>コードの更新

`:::code`Markdown で使用される構文は、ソース コード ファイル内の特定のコメントによって異なります。 これらのコメントは次のようになります。

```csharp
// <MySnippet>
Console.WriteLine("Hello World!");
// </MySnippet>
```

これらの "マーカー" コメントの間でコードを更新すると、Microsoft のドキュメント サイトに公開された場合、Markdown ファイルは自動的にこれらの変更Graphされます。 これらのコメント以外のコードを更新する場合は、対応する Markdown を更新する必要がある可能性が非常に高い。

## <a name="adding-features"></a>機能の追加

熱意が高く評価される一方で、サンプルに新機能を追加するためにプル要求を送信しないで下さい。 このリポジトリは主に"最初のアプリをビルドする" チュートリアルなので、機能セットは設計上制限されています。

## <a name="submitting-pull-requests"></a>プル要求の送信

すべてのプル要求をブランチに送信 `master` してください。

## <a name="when-do-changes-get-published"></a>変更が公開されるのは、いつですか?

Microsoft のチュートリアル サイトへの更新[プログラムGraphは](https://docs.microsoft.com/graph/tutorials)自動的には発行しません。 変更を最初にブランチに昇格してから、サイト管理者がビルド `live` をトリガーする必要があります。 これは通常、"必要に応じて" ベースで行われます。

## <a name="code-of-conduct"></a>Code of conduct

このプロジェクトでは、[Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/) が採用されています。詳細については、「[規範に関する FAQ](https://opensource.microsoft.com/codeofconduct/faq/)」を参照してください。または、その他の質問やコメントがあれば、[opencode@microsoft.com](mailto:opencode@microsoft.com) までにお問い合わせください。
