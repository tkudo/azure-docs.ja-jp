Azure Portal を使用して Resource Manager デプロイメント モデルで VNet を作成するには、次の手順に従います。 スクリーンショットは例として示されています。 サンプルの値は必ず実際の値に変更してください。 仮想ネットワークの操作の詳細については、「 [仮想ネットワークの概要](../articles/virtual-network/virtual-networks-overview.md)」を参照してください。

1. ブラウザーから [Azure Portal](http://portal.azure.com) に移動します。必要であれば Azure アカウントでサインインします。
2. **[新規]**をクリックします。 **[Marketplace を検索]** フィールドに「仮想ネットワーク」と入力します。 検索結果の一覧から **[仮想ネットワーク]** を探してクリックし、**[仮想ネットワーク]** ブレードを開きます。
   
    ![Locate Virtual Network resource blade](./media/vpn-gateway-basic-vnet-rm-portal-include/newvnetportal700.png "Locate virtual network resource blade")
3. [仮想ネットワーク] ブレードの下の方にある **[デプロイ モデルの選択]** の一覧で、**[リソース マネージャー]** を選択し、**[作成]** をクリックします。

    ![Select Resource Manager](./media/vpn-gateway-basic-vnet-rm-portal-include/resourcemanager250.png "Select Resource Manager")

1. **[仮想ネットワークの作成]** ブレードで、VNet の設定を構成します。 フィールドへの入力時、文字が有効であれば、赤色の感嘆符が緑色のチェック マークに変わります。
   
    ![Field validation](./media/vpn-gateway-basic-vnet-rm-portal-include/checkmark300.png "Field validation")
2. **[仮想ネットワークの作成]** ブレードは、次のようになっています。 自動的に入力される値もあります。 そのような値については、実際の値に変更してください。
   
    ![仮想ネットワーク ブレードの作成](./media/vpn-gateway-basic-vnet-rm-portal-include/createvnet300.png "Create virtual network blade")
3. **[名前]**: 仮想ネットワークの名前を入力します。
4. **[アドレス空間]**: アドレス空間を入力します。 追加するアドレス空間が複数ある場合は、1 つ目のアドレス空間を追加してください。 その他のアドレス空間は後で、VNet を作成した後に追加できます。
5. **[サブネット名]**: サブネットの名前とアドレス範囲を追加します。 その他のサブネットは後で、VNet を作成した後に追加できます。
6. **[サブスクリプション]**: 一覧表示されているサブスクリプションが正しいことを確認します。 ドロップダウンを使用して、サブスクリプションを変更できます。
7. **[リソース グループ]**: 既存のリソース グループを選択するか、新しいリソース グループの名前を入力して新しく作成します。 新しいグループを作成する場合は、計画した構成値に基づいて、リソース グループに名前を付けます。 リソース グループの詳細については、「 [Azure リソース マネージャーの概要](../articles/azure-resource-manager/resource-group-overview.md#resource-groups)」を参照してください。
8. **[場所]**: VNet の場所を選択します。 この場所の設定によって、この VNet にデプロイしたリソースの配置先が決まります。
9. ダッシュボードで VNet を簡単に検索できるようにするには、**[ダッシュボードにピン留めする]** を選択します。その後、**[作成]** をクリックします。
   
   ![Pin to dashboard](./media/vpn-gateway-basic-vnet-rm-portal-include/pintodashboard150.png "pin to dashboard")
10. **[作成]** をクリックした後で、VNet の進捗状況を反映するタイルがダッシュボードに表示されます。 タイルは、VNet の作成が進むに従って変化します。
    
    ![仮想ネットワーク タイルの作成](./media/vpn-gateway-basic-vnet-rm-portal-include/deploying150.png "Creating virtual network tile")

