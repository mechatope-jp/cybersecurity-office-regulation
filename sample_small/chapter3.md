#	情報資産管理
## 適用範囲 全社・全従業員

1. 情報資産の管理

    1.1 情報資産の特定と機密性の評価
    当社事業に必要で価値がある情報及び個人情報（以下「情報資産」という）を特定し、「情報資産管理台帳」に記載する。情報資産の機密性は、以下の基準に従って評価する。情報セキュリティ部門責任者は、四半期に一度、各部門で取り扱うデータ内容の点検を行い、情報資産管理台帳の更新を行う。

    <table>
        <tr>
            <td>機密性2：極秘</td><td> - 法律で安全管理が義務付けられている  <br> - 守秘義務の対象として指定されている <br> - 限定提供データ（一定の条件を満たす特定の外部者に提供することを目的とする情報）として指定されている <br> - 営業秘密（秘密として管理されているもの）として指定されている <br> - 漏えいすると取引先や顧客に大きな影響がある</td>
        </tr>
        <tr>
            <td>機密性1：社外秘</td><td>漏えいすると事業に大きな影響がある</td>
        </tr>
        <tr>
            <td>機密性0：公開</td><td>漏えいしても事業にほとんど影響はない</td>
        </tr>
    </table>

    1.2 情報資産の分類の表示
    情報資産の機密性は以下の方法で表示する。
    - 電子データ：保存先サーバーのフォルダー名に表示？？？？？？？
    - 書類：保管先キャビネット、ファイル、バインダーに表示
    表示が困難な場合は、「情報資産管理台帳」に機密性評価値を表示する。

    1.3 情報資産の管理責任者
    情報資産の取り扱い関する情報セキュリティの運用管理責任者は、当該情報資産を利用する部門長（情報セキュリティ部門責任者）とする。

    1.4 情報資産の利用者
    情報資産の利用者の範囲は、「情報資産管理台帳」の利用者範囲欄に示された部門に従事する従業員とする。

2. 情報資産の社外持ち出し
情報資産を社外に持ち出す場合には、以下を実施する。
- 社外秘の場合は所属部門長の許可を得る。
- 極秘の場合は代表取締役の許可を得る。
- ノートパソコンのハードディスクに保存して持ち出す場合は、ハードディスク/フォルダー/データを暗号化する。
- スマートフォン、タブレットに保存して持ち出す場合は、セキュリティロックを設定する。
- USBメモリ、HDD等の電子媒体に保存して持ち出す場合は、不要データは全て完全消去専用ツールで消去し、持ち出すデータを暗号化する。
- USBメモリ等の小型電子媒体は、大きなタグを付け、落としてもすぐに分かるように鈴を付ける。
- 屋外でネットワークへ接続して極秘又は社外秘の情報資産を送受信する場合は、暗号化する。
- 携行中は常に監視可能な距離を保つ。

3. 媒体の処分

    3.1 媒体の廃棄
    社外秘又は極秘の情報資産を廃棄する場合は以下の処分を行う。

    <table>
    <tr>
        <td>書類・フィルム</td><td>細断ののち溶解または焼却</td>
    </tr>
    <tr>
        <td>USBメモリ</td><td>破壊による完全消去 <br> ※OSによる削除・クイックフォーマットは不可/td>
    </tr>
    <tr>
        <td>HDD・CD・DVD</td><td>破壊または細断による完全消去 <br> ※OSによる削除・クイックフォーマットは不可/td>
    </tr>
    </table>

    3.2 媒体の再利用
    極秘又は社外秘の情報資産を保存した媒体を再利用する場合は、以下の処分を行う。

    <table>
    <tr>
        <td>書類</td><td>裏紙再利用禁止</td>
    </tr>
    <tr>
        <td>USBメモリ・HDD・CD-RWディスク・DVD-RWディスク</td><td>完全消去後再利用 <br> ※OSによる削除・クイックフォーマットは不可？？？？？？？</td>
    </tr>
    <tr>
        <td>CD-R・DVD-R</td><td>再利用不可</td>
    </tr>
    </table>

4. バックアップ

    4.1 バックアップ取得対象？？？？？？？
    情報システム管理者は、以下の機器で処理するデータのバックアップを定期的に取得する。

    | 機器名 | 対象 | 方法 | 保管先 |
    | --- | --- | --- | --- |
    | ファイルサーバー | ユーザーファイル | Windows Server バックアップ | NASサーバー |
    | 給与計算システム | アプリケーションデータ | ファイルコピー | 専用外付けHDD（暗号化機能付） |
    | 会計システム | アプリケーションデータ | アプリケーションバックアップ機能 | クラウドバックアップサービス |
    | ○○管理システム | アプリケーションデータ | 同期ツール | 外付けHDD |
    | Webサーバー | ホームページ | 同期ツール | NASサーバー |

    4.2 バックアップ媒体の取り扱い
    バックアップに利用した機器及び媒体の取り扱いは以下に従う。
    ＜保管＞
    - 小型媒体：施錠付きキャビネットに保管
    - NASサーバー：施錠付きサーバーラックに収納
    ＜廃棄・再利用＞
    - 「3.媒体の処分」に従う

    4.3 クラウドサービスを利用したバックアップ
    クラウドサービスを利用し、外部のサーバーにバックアップを保存する場合は、以下のサービス要件を確認し、情報セキュリティ部門責任者の許可を得て導入する。
    ＜サービス要件＞
    - サービス提供者のサービス利用約款、情報セキュリティ方針が、当社の情報セキュリティ関連規程に適合している。
    - 当社事業所がある地域で発生する震災、水害等の影響を受けない地域の施設であること。