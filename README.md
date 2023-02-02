## Memo
- `bin/cdk-{project}.ts`
  - CDK アプリケーションへのエントリポイント
  - これによって`lib/*`で定義したすべてのスタックがロード/作成される
- `lib/cdk-{project}-stack.ts`
  - メインの CDK アプリケーションスタックが定義
  - リソースとそのプロパティはここに含める
- `package.json`
  - プロジェクトの依存関係、およびいくつかの追加情報とビルドスクリプト (npm build、npm test、npm watch) を定義
- `cdk.json`
  - アプリケーションの実行方法、および CDK とプロジェクトに関連する追加設定とパラメータをツールキットに指示

# Welcome to your CDK TypeS
This is a blank project for CDK development with TypeScript.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

## Useful commands

* `npm run build`   compile typescript to js
* `npm run watch`   watch for changes and compile
* `npm run test`    perform the jest unit tests
* `cdk deploy`      deploy this stack to your default AWS account/region
* `cdk diff`        compare deployed stack with current state
* `cdk synth`       emits the synthesized CloudFormation template
