## ユーザー空間

ユーザー空間にトランスポートプロトコルを実装することで、プロトコルの開発サイクルを速めることができます。これは、クライアントとサーバー OS のカーネルをアップデートすることなくプロトコルの更新を比較的簡単に行えるためです。

技術的には、QUIC 固有の仕組みをユーザー空間ではなくカーネル空間にて実装することも可能です。一部の開発者にとってはそのほうが都合が良いこともあるでしょう。

### 多数の実装

ユーザースペースに新しいトランスポートプロトコルを実装する明らかな効果は、独立した実装を多数期待できることです。

将来、種々のアプリケーションは異なる HTTP/3 や QUIC の実装を取り込むことが(最上層に実装することも)起こりうるでしょう。