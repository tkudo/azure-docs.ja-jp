---
title: "Azure Active Directory B2B コラボレーションのライセンスに関するガイダンス | Microsoft Docs"
description: "Azure Active Directory B2B コラボレーションでは、B2B コラボレーション ユーザー用に必要な機能に応じて、Azure AD 有料ライセンスが必要となります。"
services: active-directory
documentationcenter: 
author: sasubram
manager: femila
editor: 
tags: 
ms.assetid: 
ms.service: active-directory
ms.devlang: NA
ms.topic: article
ms.tgt_pltfrm: NA
ms.workload: identity
ms.date: 05/23/2017
ms.author: sasubram
ms.translationtype: Human Translation
ms.sourcegitcommit: 7f469fb309f92b86dbf289d3a0462ba9042af48a
ms.openlocfilehash: 4e620f3d76caa25ac0e5afb134f37ffe263935f0
ms.contentlocale: ja-jp
ms.lasthandoff: 04/13/2017


---

# <a name="azure-active-directory-b2b-collaboration-licensing-guidance"></a>Azure Active Directory B2B コラボレーションのライセンスに関するガイダンス

Azure Active Directory (Azure AD) B2B コレボレーションでは、選択された既存の Azure AD 機能セットが、Azure AD テナントに招待されたゲスト ユーザーにも適用されます。 そのため、Azure AD B2B コラボレーションのゲスト ユーザーは、Azure AD ライセンスによって使用許諾され、https://azure.microsoft.com/pricing/details/active-directory/ に示すように、既存の Free、Basic、Premium P1/P2 の各ライセンス レベルに従うことになります。

B2B ユーザーを招待し、Azure AD でアプリケーションに割り当てる際に料金は発生しません。 また、B2B ユーザーは、ゲスト ユーザーごとに最大 10 個のアプリと 3 つの基本レポートも無料で利用できます。これらは、Azure AD の "Free" レベルに含まれるためです。
B2B コラボレーション機能によって B2B ユーザーにも適用される Azure AD の有料機能は、Azure AD 有料ライセンス (使用する機能に応じて、Basic、Premium P1、または Premium P2) によって使用を許諾する必要があります。 招待元のテナントは、Azure AD 有料ライセンスごとに 5 人の B2B ユーザーの権利を取得します。 つまり、Azure AD 有料機能に対する権利を、テナントの 1 人の従業員ユーザーに付与する各 Azure AD 有料ライセンスでは、その Azure AD 有料機能に対する権利が、テナントに招待された 5 人の追加 B2B ユーザーにも付与されます。

## <a name="licensing-examples"></a>ライセンスの例
- お客様が 100 人の B2B ユーザーを Azure AD テナントに招待したいと考えています。このすべてのユーザーに対してグループ ベースのアクセス管理とプロビジョニングを使用しますが、50 人のユーザーには MFA と条件付きアクセスも必要となります。 このお客様の場合、すべての B2B ユーザーに適切に対応するには、10 個の Azure AD Basic ライセンスと 10 個の Azure AD Premium P1 ライセンスを購入する必要があります。 同様に、招待元のテナントが B2B ユーザーに対して Identity Protection の機能を使用する場合、5:1 の比率ですべての B2B ユーザーに対応できる十分な数の Azure AD Premium P2 ライセンスが必要となります。
- お客様には、現在 Azure AD Premium P1 ライセンスが付与された 10 人の従業員がいます。 これらの従業員は、60 人の B2B ユーザーを招待する必要があり、すべてのユーザーに Multi-Factor Authentication (MFA) が必要となります。 5:1 のライセンス ルールに従い、このお客様が全 60 人の B2B コラボレーション ユーザーに対応するには、少なくとも 12 個の Azure AD Premium P1 ライセンスが必要です。 10 人の従業員の 10 個の Premium P1 ライセンスが既にあるため、MFA などの Premium P1 の機能を使用する 50 人の B2B ユーザーを招待する権利が既にあります。 したがって、この例では、残りの 10 人の B2B コラボレーション ユーザーに対応するために、Premium P1 ライセンスをあと 2 つ購入する必要があります。

> [!NOTE]
> これらの B2B コラボレーション ユーザーの権利を有効にするために、B2B ユーザーにライセンスを割り当てる手段はなく、その必要もありません。

招待元のテナントを所有するお客様が、Azure AD の有料機能を必要とする B2B コラボレーション ユーザーの数を判断する必要があります。また、必要な機能が、Basic、Premium P1、Premium P2 のどのレベルの機能であるかに応じて、5:1 の比率で B2B コラボレーション ユーザーに対応できる十分な数の適切な Azure AD 有料ライセンスが必要となります。 会社で B2B コラボレーション ユーザーの権利がさらに必要な場合は、必要な Azure AD 有料ライセンスを購入する必要があります。

## <a name="additional-licensing-details"></a>ライセンスのその他の詳細
- B2B コラボレーションでは、Azure AD のエディションの既存のモデルに基づいて、B2B コラボレーション ユーザーごとにそれぞれ異なる機能を提供できます。
- 各 Azure AD 有料ライセンスには、5 人の B2B コラボレーション ユーザーの権利が含まれます (5:1 モデル)。
- B2B ユーザー アカウントにライセンスを実際に割り当てる必要はありません。 自動的に計算され、報告されます。
- テナントに Azure AD 有料ライセンスがない場合、招待された各ユーザーは、Azure AD Free エディションで提供される権利を取得します。
- B2B コラボレーション ユーザーが、自分の組織の従業員として Azure AD 有料ライセンスを持っている場合、招待元のテナントの B2B コラボレーション ライセンスは使用されません。

## <a name="advanced-discussion-what-are-the-licensing-considerations-when-we-add-users-from-a-conglomerate-organization-as-members-using-your-apis"></a>高度なディスカッション: 貴社の API を使用して複合組織からユーザーを「メンバー」として追加する際のライセンスに関する考慮事項は何ですか?
B2B ゲスト ユーザーとは、パートナー組織から招待されてホスト組織で仕事をするユーザーです。 一般に、これ以外のケースでは、B2B 機能を使用しても B2B とはみなされません。 具体的に 2 つのケースを見てみましょう。

1. ホストがコンシューマー アドレスを使用して従業員を招待する場合
  1. これはライセンス ポリシーに準拠しておらず、現在は推奨できません。

2. ホスト組織が別の複合組織からユーザーを追加する場合
  1. このケースでユーザーは B2B API を使用して招待されますが、これは従来型の B2B ではありません。 理想として、これらの組織は他の組織ユーザーをメンバーとして招待するべきです (当社の API もこれなら可能です)。 この場合、これらのメンバーにライセンスを割り当てて、招待側組織のリソースにアクセスできるようにしなければなりません。

  2. 組織の中には、他の組織のユーザーをポリシー上「ゲスト」として追加したい場合もあるでしょう。 次の 2 つのケースがあります。
      * 複合組織がすでに Azure AD を使用しており、招待されたユーザーが他の組織でライセンスを与えられている: この場合、招待されたユーザーは本書で既出の 1:5 の式に従う必要はありません。 

      * 複合組織が Azure AD を使用していないか、適切なライセンスを持っていない: この場合は、このドキュメントで既出の 1:5 の式に従います。


## <a name="next-steps"></a>次のステップ

Azure AD B2B コラボレーションに関する他の記事を参照してください。

* [Azure AD B2B コラボレーションとは](active-directory-b2b-what-is-azure-ad-b2b.md)
* [Azure Active Directory 管理者が B2B コラボレーション ユーザーを追加する方法](active-directory-b2b-admin-add-users.md)
* [インフォメーション ワーカーが B2B コラボレーション ユーザーを追加する方法](active-directory-b2b-iw-add-users.md)
* [B2B コラボレーションの招待メールの要素](active-directory-b2b-invitation-email.md)
* [B2B コラボレーションの招待の利用](active-directory-b2b-redemption-experience.md)
* [Azure Active Directory B2B コラボレーションのトラブルシューティング](active-directory-b2b-troubleshooting.md)
* [Azure Active Directory B2B コラボレーションに関してよく寄せられる質問 (FAQ)](active-directory-b2b-faq.md)
* [Azure Active Directory B2B コラボレーションの API とカスタマイズ](active-directory-b2b-api.md)
* [B2B コラボレーション ユーザーの多要素認証](active-directory-b2b-mfa-instructions.md)
* [招待を使用せずに B2B コラボレーション ユーザーを追加する](active-directory-b2b-add-user-without-invite.md)
* [Article Index for Application Management in Azure Active Directory](active-directory-apps-index.md)

