---

copyright:
  years: 2017
lastupdated: "2017-12-05"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}

# チャネルの作成または更新

チャネルは、データのパーティショニングおよび分離のための非常に強力なメカニズムであり、データのプライバシーのための主要な基盤を提供します。同じチャネルのメンバーだけが、このチャネルのデータにアクセスできます。
{:shortdesc}

チャネルのセキュリティーを確保するために、チャネル更新のポリシーが構成されて、
チャネルを作成または更新する前にチャネルの作成または更新の要求に同意する必要のあるチャネル・オペレーターの数が定義されています。
 

## チャネルの作成
ネットワーク・モニターの「チャネル (Channels)」画面で**「新規チャネル (New Channel)」**ボタンをクリックし、以下のステップを実行してチャネル作成要求を送信します。  
1. チャネルのビジネス目標を反映する名前を選択し、必要に応じて説明を追加し、**「次へ」**をクリックします。チャネル名はブロックチェーン・ネットワーク内で固有のものでなければなりません。この先頭は文字でなければならず、小文字、数字、ダッシュだけを含めることができます。  
  ![チャネルの作成 1](../images/create_channel.png "チャネルの作成パネル 1")  
    
2. ネットワーク・メンバーを選択してから**「メンバーの追加 (Add Member)」**ボタンをクリックすることによって、任意の組み合わせのネットワーク・メンバーを招待します。招待した各メンバーに役割を割り当てることによって許可をカスタマイズしてから、**「次へ」**をクリックします。  
  ![チャネルの作成 2](../images/create_channel_2.png "チャネルの作成パネル 2")  
  
    * チャネル・オペレーターは、チャネル台帳を照会または更新することができます。チャネル・オペレーターには、チャネル作成要求を**受諾**または**拒否**する権限とチャネル更新要求を送信する権限があります。各チャネルには、最低でも 1 名の**オペレーター**が必要です。  
    * チャネル・ライターは、チャネル台帳を更新できます。
    * チャネル・リーダーは、チャネル台帳の照会だけを行うことができます。
  
3. チャネル更新要求の承認に必要なチャネル・オペレーターの数を選択してチャネル更新ポリシーを構成してから、**「要求の実行依頼 (Submit Request)」**をクリックします。   
  ![チャネルの作成 3](../images/create_channel_3.png "チャネルの作成パネル 3")  

招待されたメンバーは、招待メールを受け取ります。また、ネットワーク・モニターの**「通知」**画面の「すべて」または「処理待ち」サブタブに要求が表示されます。  
* チャネル・オペレーターとして招待されたメンバーは**「要求の確認 (Review Request)」**ボタンをクリックしてチャネル構成を確認してから、要求を**受諾**または**拒否**することができます。「マイ・ステータス (My Status)」列に、要求に対するオペレーターの投票状況が表示されます。
    * _投票の処理待ち (Vote Pending)_: オペレーターが要求を処理していない。
    * _投票受諾 (Vote Accepted)_: オペレーターが要求を受け入れた。
    * _投票拒否 (Vote Declined)_: オペレーターが要求を却下した。
    * _投票クローズ済み (Vote Closing)_: 要求が十分な**受諾**投票を得て、オペレーターが受諾または拒否を行う必要がなくなった。
* チャネル・ライターまたはリーダーとして招待されたメンバーには、「マイ・ステータス (My Status)」列に*「不要 (Not Required)」*が表示されます。要求に対してチャネル・オペレーターから十分な**受諾**投票が得られる前は、ライターまたはリーダーが**「要求の確認 (Review Request)」**ボタンをクリックしてチャネル構成を確認することができます。

十分な数のチャネル・オペレーターが要求を承認した場合、任意のチャネル・メンバーが**「要求の実行依頼 (Submit Request)」**ボタンをクリックすると、新規チャネルが作成されます。すべてのチャネル・メンバーは、ネットワーク・モニターの「チャネル(Channels)」画面でそのチャネルを確認できます。

## チャネルの更新
チャネル・メンバーの追加や削除またはチャネル更新ポリシーの変更など、チャネルの構成を変更する場合は、チャネル更新要求を送信できます。ネットワーク・モニターの「チャネル (Channels)」画面で、変更するチャネルを見つけた後に、**「アクション」**ヘッダーの下にあるドロップダウン・リストから**「チャネルの編集 (Edit Channel)」**を選択します。パネル内をナビゲートして必要なエンティティーを変更し、**「要求の実行依頼 (Submit Request)」**をクリックしてチャネル更新要求を開始します。

すべてのチャネル・メンバーは、チャネル更新要求に関する電子メール通知を受け取ります。
* 新しく招待されたメンバーは、チャネルに参加するように招待する電子メール通知を受け取ります。さらに、ネットワーク・モニターの**「通知」**画面に「投票の処理待ち (Vote Pending)」状況の要求が表示されます。 
    * チャネル・オペレーターとして招待されたメンバーは**「要求の確認 (Review Request)」**ボタンをクリックしてチャネル構成を確認してから、チャネル更新要求を**受諾**または**拒否**することができます。「マイ・ステータス (My Status)」列に、要求に対するオペレーターの投票状況が表示されます。
        * _投票の処理待ち (Vote Pending)_: オペレーターが要求を処理していない。
        * _投票受諾 (Vote Accepted)_: オペレーターが要求を受け入れた。
        * _投票拒否 (Vote Declined)_: オペレーターが要求を却下した。
        * _投票クローズ済み (Vote Closing)_: 要求が十分な**受諾**投票を得て、オペレーターが受諾または拒否を行う必要がなくなった。
    * チャネル・ライターまたはリーダーとして招待されたメンバーには、「マイ・ステータス (My Status)」列に*「不要 (Not Required)」*が表示されます。要求に対してチャネル・オペレーターから十分な**受諾**投票が得られる前は、ライターまたはリーダーが**「要求の確認 (Review Request)」**ボタンをクリックしてチャネル構成を確認することができます。
* 削除されたメンバーは、チャネルの変更に関する電子メール通知を受け取ります。
* 既存のチャネル・オペレーターは、チャネルの更新に関する電子メール通知を受け取ります。ネットワーク・モニターの**「通知」**画面に_「投票の処理待ち (Vote Pending)」_状況の要求が表示され、その**受諾**または**拒否**を行うことができます。
* 既存のチャネル・ライターまたはリーダーも、チャネルの更新に関する電子メール通知を受け取ります。ネットワーク・モニターの**「通知」**画面に_「不要 (Not Required)」_状況の要求が表示されます。

十分な数のチャネル・オペレーターが要求を承認した場合、任意のチャネル・メンバーが**「要求の実行依頼 (Submit Request)」**ボタンをクリックすると、チャネルが更新されます。すべてのチャネル・メンバーは、ネットワーク・モニターの「チャネル(Channels)」画面で更新されたチャネルを確認できます。
