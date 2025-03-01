---
lab:
  title: 'ラボ 3.1: 製品カタログを構成する'
---

# モジュール 3: Dynamics 365 を使用して注文と製品カタログを管理する

## 実習ラボ 3.1 - 製品カタログを管理する

### シナリオ
Contoso Coffee は成長に伴い、価格構造を標準化し、より正確な価格と製品の詳細を使用して見積もり、注文、請求書をより簡単に作成できるようにすることを検討しています。 Contoso Coffee は最近、最新のスマート コーヒー マシンを発売しました。 Dynamics 365 Sales 実装の業務コンサルタントとして、あなたは製品カタログの構成を依頼されています。

このラボをきちんと修了すると、次のことができるようになります。
- 出荷単位一覧の作成
- 価格表の定義
- 割引表の作成
- 製品および製品ファミリの定義

### 演習 1 - 製品カタログ

#### タスク 1 - 出荷単位一覧を作成する
このタスクでは、コーヒー マシン フィルターのラインナップの出荷単位一覧を作成します。
1. Dynamics 365 営業ハブ アプリケーションに移動します。
2. [変更] 領域メニュー (画面の左下にあります) をクリックします。 既定では、[Sales] は左側のメニューの下部に表示されます。
3. 表示されるメニューから**アプリの設定**を選択します。
4. 左側メニューの [製品カタログ] セクションから **[出荷単位一覧]** を選択します。
5. **[+ 新規]** をクリックします。
6. [名前] に「**フィルター**」と入力し、標準出荷単位に「**それぞれ**」と入力し、**[OK]** をクリックします。
7. 出荷単位一覧が開いたら、[関連] タブを選択し、**[単位]** を選択します。
8. 既定の単位 "それぞれ" のみが表示されていて、さらに 3 つの単位を追加します。 **[+ 新しい単位]** をクリックします。
9. [名前] に「<bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</bpt></bpt>フィルター<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">*</ept></ept>」、[数量] に「<bpt ctype="x-unknown" id="3" rid="2"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</bpt></bpt>1<ept id="4" rid="2"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p2">*</ept></ept>」と入力し、[基本単位] に <bpt ctype="x-unknown" id="5" rid="3"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</bpt></bpt>[それぞれ]<ept id="6" rid="3"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p3">**</ept></ept> を選択し、[保存して閉じる] ボタンの右側にある <bpt ctype="x-unknown" id="9" rid="5"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</bpt></bpt>[˅]<ept id="10" rid="5"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p5">**</ept></ept> ドロップダウン アイコンを選択して<bpt ctype="x-unknown" id="7" rid="4"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</bpt></bpt>[保存して新規作成]<ept id="8" rid="4"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p4">**</ept></ept> をクリックします。
10. [名前] に「*パック*」、[数量] に「*2*」と入力し、[基本単位] に **[フィルター]** を選択して、**[保存して新規作成]** をクリックします。
11. [名前] に「*バリュー パック*」、[数量] に「*2*」と入力し、[基本単位] に **[パック]** を選択して、**[保存して閉じる]** をクリックします。
12. これで、一覧に 4 つの出荷単位一覧ができたはずです。

#### タスク 2 - 割引表を作成する
このタスクでは、15 個、20 個またはそれ以上のフィルターを購入する顧客用の割引表を作成します。 フィルター 15 個では 15% の割引が適用され、フィルター 20 から 50 個では 25% の割引が適用されます。
1. 左側メニューの [製品カタログ] セクションから **[割引表]** を選択します。
2. **[+ 新規]** をクリックします。
3. [名前] に「*数量割引*」と入力し、[種類] に **[パーセント]** を選択し、**[保存]** をクリックします。
4. **[関連]** をクリックし、**[割引]** を選択します。
5. **[+ 新しい割引]** をクリックします。
6. 必ず [割引の種類] に [数量割引] を選択し、[開始数量] に「*15*」、[終了数量] に「*19*」、[パーセント] に「*15*」と入力して、**[保存]** をクリックします。
7. **+ 新規**をもう一度クリックします。
8. [割引の種類] に **[数量割引]** を選択します。 次に、[開始数量] に「*20*」、[終了数量] に「*50*」と入力し、[パーセント] に「*25*」と入力して、**[保存]** をクリックします。

#### タスク 3 - 価格表を作成する
このタスクでは、フィルターの価格表を作成します。
1. 左側メニューの [製品カタログ] セクションから **[価格表]** を選択します。
2. **[+ 新規]** をクリックします。
3. [名前] に「*フィルター直接*」と入力し、[通貨] に **[米国ドル]** を選択し、**[保存して閉じる]** をクリックします。

#### タスク 4 - 製品を作成する
このタスクでは、製品を作成します。
1. **[アプリ設定]** 変更領域をクリックします。
2. **[Sales]** を選択します。
3. 左側メニューの [付帯品] セクションから **[製品]** を選択します。
4. **[製品の追加]** をクリックします。
5. [名前] に「*Airpot XL 6 か月フィルター*」と入力し、[製品 ID] に「*AXL6MF-1234*」と入力し、[出荷単位一覧] に **[フィルター]** を選択し、[既定の単位] に **[フィルター]** を選択し、[サポートされる小数点以下の桁数] に「*2*」と入力して、**[保存]** をクリックします。 (提案を受け入れるために、サポートされる小数点以下の桁数の横にある青いチェック マークを選択することが必要になる場合があります。)
6. **[追加の詳細]** タブを選択します。
7. [価格表品目] セクションの右上にある**縦の省略記号**をクリックします。 **[+ 新しい価格表品目]** をクリックします。
8. [価格表] に **[フィルター直接]** を選択し、[割引表] に **[数量割引]** を選択し、[端数売り] に **[整数]** を選択します。
9. **[価格情報]** タブを選択し、[金額] に「*25*」と入力して、**[保存して閉じる]** を選択します。
10. 自動発行が有効になっている場合は、この手順をスキップします。 ([発行] はコマンド バーに表示されません。) それ以外の場合は、**[発行]**、**[確認]** の順に選択して製品を発行します。
11. 左側のメニューで、[付帯品] グループの **[製品]** を選択します。
12. **[製品の追加]** をクリックします。
13. [名前] に「*Airpot XL Reservoir エクステンション*」と入力し、[製品 ID] に「*AXLRE-4321*」と入力し、[出荷単位一覧] に **[既定の単位]** を選択し、[既定の単位] に **[標準出荷単位]** を選択し、[サポートされる小数点以下の桁数] に対する 2 の横にある青いチェックマークを選択して、**[保存]** をクリックします。
14. **[追加の詳細]** タブを選択します。
15. [価格表品目] セクションの右上にある**縦の省略記号**をクリックします。 **[+ 新しい価格表品目]** をクリックします。
16. [価格表] に **[フィルター直接]** を選択します。 [端数売り] に **[整数]** を選択します。
17. **[価格情報]** タブを選択し、[金額] に「*299 ドル*」と入力して、**[保存して閉じる]** を選択します。
18. 自動発行が有効になっている場合は、この手順をスキップします。 それ以外の場合は、**[発行]**、**[確認]** の順に選択して製品を発行します。
19. 左側のメニューで **[製品]** を選択します。
20. **[製品の追加]** をクリックします。
21. [名前] に「*Airpot XL Pot エクステンダー*」と入力し、[製品 ID] に「*AXPLE-7894*」と入力し、[出荷単位一覧] に **[既定の単位]** を選択し、[既定の単位] に **[標準出荷単位]** を選択し、[サポートされる小数点以下の桁数] に対する 2 の横にある青いチェック マークを選択して、**[保存]** をクリックします。
22. **[追加の詳細]** タブを選択します。
23. [価格表品目] セクションの右上にある**縦の省略記号**をクリックします。 **[+ 新しい価格表品目]** をクリックします。
24. [価格表] に **[フィルター直接]** を選択します。 [端数売り] に **[整数]** を選択します。
25. **[価格情報]** タブを選択し、[金額] に「*199*」と入力して、**[保存して閉じる]** を選択します。
26. 自動発行が有効になっている場合は、この手順をスキップします。 それ以外の場合は、**[発行]**、**[確認]** の順に選択して製品を発行します。
27. 左側のメニューで **[製品]** を選択します。
28. 作成した製品は、[すべての製品] の [ファミリとバンドル] ビューに表示されるはずです。 既定ビューのタイトルの横にある <bpt ctype="x-unknown" id="1" rid="1"><bpt xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</bpt></bpt>[˅]<ept id="2" rid="1"><ept xmlns="urn:oasis:names:tc:xliff:document:1.2" id="p1">**</ept></ept> ドロップダウン アイコンを選択することで、このビューに切り替えることができます。 
