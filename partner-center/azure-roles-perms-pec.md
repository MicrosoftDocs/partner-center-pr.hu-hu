---
title: Szerepkörök, partner által létrehozott kreditek
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ismerje meg, hogy a partnerek milyen szerepkörökkel és engedélyekkel szerezhetik be a partner által szerzett krediteket (PEC). Ezek eltérnek a partner Centerben működő szerepköröktől.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8c36883dc7d12b7ea0ce8f2644dbac86595ab131
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: hu-HU
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534590"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>A partner által szerzett kreditek megszerzéséhez szükséges szerepkörök és engedélyek

A következő szerepkörök az engedélyek szintjeire mutatnak, amelyek meghatározzák, hogy a partnerek jogosultak-e a partner által létrehozott kreditek használatára.

>[!Important]
>Ezek a szerepkörök és engedélyek nem egyeznek meg azokkal a szerepkörökkel és engedélyekkel, amelyeket a felhasználónak a partner Centerben kell működnie.

|**Szerepkör**   |**Leírás**   |**PEC jogosult**   |
|-----------------|:------------------|:--------------|
|Tulajdonos  |Mindent kezel, beleértve az erőforrásokhoz való hozzáférést is.|Igen|
|Közreműködő |Mindent kezel, kivéve az erőforrásokhoz való hozzáférés biztosítását.|Igen|
|Olvasó|Mindent megtekintheti, de nem végezheti el a módosításokat|Nem|
|ACRDelete|ACR törlése|Igen|
|ACRImageSigner|ACR-rendszerkép aláírója|Igen|
|ACRPull|ACR-lekérés|Igen|
|AcrPush|ACR leküldése|Igen|
|AcrQuarantineReader|ACR karanténba helyezési Adatolvasó|Nem|
|AcrQuarantineWriter| az ACR karanténba helyezési adatírója|Igen|
|API Management szolgáltatás közreműködői|Képes a szolgáltatás és az API-k kezelésére|Igen|
|API Management Service operátori szerepkör|Kezelheti a szolgáltatást, de nem az API-kat|Igen|
|API Management szolgáltatás-olvasó szerepkör|Csak olvasási hozzáférés a szolgáltatáshoz és az API-khoz|Nem|
|Application Insights összetevő közreműködője|Application Insights összetevőket felügyel|Igen|
|Application Insights Snapshot Debugger|Felhasználói jogosultságot biztosít a Application Insights Snapshot Debugger gyűjtött hibakeresési Pillanatképek megtekintéséhez és letöltéséhez. Vegye figyelembe, hogy ezek az engedélyek nem szerepelnek a tulajdonos vagy a közreműködő szerepkörben.|Igen|
Automation-feladatok operátora | Feladatok létrehozása és kezelése Automation-Runbookok használatával. | Igen | 
Automation-operátor | Az Automation-operátorok képesek a feladatok elindítására, leállítására, felfüggesztésére és folytatására | Igen | 
Automation Runbook operátor | A Runbook tulajdonságainak olvasása – a Runbook feladatai létrehozásához. | Igen | 
Avere közreműködője | Létrehozhat és kezelhet egy avere vFXT-fürtöt. | Igen | 
Avere operátor | A avere vFXT-fürt által használt fürt kezelése | Igen | 
Az Azure Event Hubs adattulajdonos | Lehetővé teszi az Azure Event Hubs-erőforrások teljes hozzáférését. | Igen | 
Azure Event Hubs adatfogadó | Engedélyezi az Azure Event Hubs-erőforrások elérését. | Igen | 
Azure Event Hubs adatfeladó | Engedélyezi az Azure Event Hubs-erőforrásokhoz való hozzáférés küldését. | Igen | 
Azure Kubernetes Service-fürt rendszergazdai szerepköre | A fürt rendszergazdai hitelesítő adatainak listázása művelet. | Igen | 
Azure Kubernetes Service-fürt felhasználói szerepköre | Fürt felhasználói hitelesítő adatainak listázása. | Igen | 
Azure Maps Adatolvasó (előzetes verzió) | Hozzáférést biztosít egy Azure Maps-fiókból az olvasási leképezéssel kapcsolatos adatokhoz. | Nem | 
Azure Service Bus adattulajdonos | Teljes hozzáférés engedélyezése Azure Service Bus erőforrásokhoz. | Igen | 
Adatfogadó Azure Service Bus | Engedélyezi a hozzáférést Azure Service Bus erőforrásokhoz. | Igen | 
Adatfeladó Azure Service Bus | Lehetővé teszi a Azure Service Bus erőforrásokhoz való hozzáférés küldését. | Igen | 
Azure Stack regisztrációs tulajdonos | Lehetővé teszi Azure Stack regisztrációk kezelését. | Igen | 
Biztonsági mentési közreműködő | Lehetővé teszi a Backup szolgáltatás kezelését, de nem hozhat létre tárolókat, és hozzáférést biztosíthat másoknak | Igen | 
Biztonságimásolat-felelős | Lehetővé teszi a biztonsági mentési szolgáltatások kezelését, kivéve a biztonsági mentés eltávolítását, a tár létrehozását és a másokhoz való hozzáférést. | Igen | 
Backup-olvasó | Megtekintheti a biztonsági mentési szolgáltatásokat, de nem végezheti el a módosításokat | Nem | 
Számlázás olvasója | Olvasási hozzáférés engedélyezése a számlázási információkhoz | Nem | 
BizTalk közreműködő | Lehetővé teszi a BizTalk Services kezelését, de azokhoz való hozzáférés nélkül. | Igen | 
Blockchain-hozzáférés (előzetes verzió) | Engedélyezi a hozzáférést a Blockchain-tagok csomópontjaihoz | Igen | 
Tervezet közreműködője | Kezelheti a terv definícióit, de nem rendelheti hozzá őket. | Igen | 
Blueprint operátor | Meglévő közzétett tervrajzokat is hozzárendelhet, de nem hozhat létre új tervrajzokat. Megjegyzés: ez csak akkor működik, ha a hozzárendelés felhasználó által hozzárendelt felügyelt identitással lett végrehajtva. | Igen | 
CDN-végpont közreműködői | Kezelheti a CDN-végpontokat, de nem tud hozzáférést biztosítani más felhasználóknak. | Igen | 
CDN-végpont olvasója | Megtekintheti a CDN-végpontokat, de nem végezheti el a módosításokat. | Nem | 
CDN-profil közreműködői | Kezelheti a CDN-profilokat és azok végpontjait, de nem adhat hozzáférést más felhasználóknak. | Igen | 
CDN-profil olvasója | Megtekintheti a CDN-profilokat és azok végpontjait, de nem végezhet módosításokat. | Nem | 
Klasszikus hálózati közreműködő | Lehetővé teszi a klasszikus hálózatok kezelését, de azokhoz való hozzáférés nélkül. | Igen | 
Klasszikus Storage-fiók közreműködői | Lehetővé teszi a klasszikus Storage-fiókok kezelését, de azokhoz való hozzáférés nélkül. | Igen | 
A klasszikus Storage-fiók kulcs-kezelő szolgáltatásának szerepköre | A klasszikus Storage-fiók kulcsfontosságú operátorai jogosultak a kulcsok listázására és újragenerálása a klasszikus Storage-fiókokban | Igen | 
Klasszikus virtuális gép közreműködője | Lehetővé teszi a klasszikus virtuális gépek kezelését, de nem fér hozzájuk, nem pedig a virtuális hálózati vagy a Storage-fiókhoz, amelyhez csatlakoznak. | Igen | 
Cognitive Services közreműködő | Lehetővé teszi Cognitive Services kulcsainak létrehozását, olvasását, frissítését, törlését és kezelését. | Igen | 
Cognitive Services Adatolvasó (előzetes verzió) | Lehetővé teszi Cognitive Services-információk olvasását. | Nem | 
Cognitive Services felhasználó | Lehetővé teszi Cognitive Services kulcsainak olvasását és listázását. | Nem | 
Cosmos DB fiók-olvasó szerepkör | Azure Cosmos DB fiókadatok olvasása. Lásd: DocumentDB Account közreműködő a Azure Cosmos DB-fiókok kezeléséhez. | Nem | 
Cosmos DB operátor | Lehetővé teszi Azure Cosmos DB-fiókok kezelését, de nem férnek hozzájuk. Megakadályozza a fiók kulcsai és a kapcsolati karakterláncok elérését. | Igen | 
CosmosBackupOperator | Visszaküldheti a visszaállítási kérelmet egy Cosmos DB adatbázishoz vagy egy fiókhoz tartozó tárolóhoz | Igen | 
Cost Management közreműködő | Megtekintheti a költségeket és kezelheti a költségek konfigurációját (pl. költségvetés, exportálás) | Igen | 
Cost Management olvasó | Megtekintheti a költségeket és a konfigurációt (például a költségvetést, az exportot) | Nem | 
Data Box közreműködő | A lehetővé teszi, hogy minden Data Box szolgáltatás alatt kezelje a hozzáférést, kivéve, ha mások számára biztosít hozzáférést. | Igen | 
Data Box olvasó | Lehetővé teszi Data Box szolgáltatás felügyeletét, kivéve a rendelés vagy a szerkesztési sorrend részleteit, és hozzáférést biztosít másoknak. | Nem | 
Data Factory közreműködő | Az adatüzemek létrehozása és kezelése, valamint a bennük található alárendelt erőforrások. | Igen | 
Data Lake Analytics fejlesztő | Lehetővé teszi a saját feladatok küldését, figyelését és kezelését, de Data Lake Analytics fiókokat nem hozhat létre vagy törölhet. | Igen | 
Adattisztító | Törölheti az elemzési adatfájlokat | Igen | 
DevTest Labs-felhasználó | Lehetővé teszi a virtuális gépek a Azure DevTest Labs való összekapcsolását, indítását, újraindítását és leállítását. | Igen | 
DNS-zóna közreműködője | Lehetővé teszi a DNS-zónák és-rekordhalmazok kezelését Azure DNSban, de nem teszi lehetővé, hogy ki férhet hozzájuk. | Igen | 
DocumentDB-fiók közreműködői | Felügyelheti Azure Cosmos DB fiókokat. Azure Cosmos DB korábbi nevén DocumentDB. | Igen | 
EventGrid EventSubscription közreműködője | Lehetővé teszi a EventGrid esemény-előfizetési műveletek kezelését. | Igen | 
EventGrid EventSubscription-olvasó | Lehetővé teszi a EventGrid esemény-előfizetések olvasását. | Nem | 
HDInsight-fürt operátora | Lehetővé teszi a HDInsight-fürt konfigurációjának olvasását és módosítását. | Igen | 
HDInsight tartományi szolgáltatások közreműködője | Elolvashatja, létrehozhatja, módosíthatja és törölheti a HDInsight kapcsolatos tartományi szolgáltatásokat Enterprise Security Package | Igen | 
Intelligens rendszer-fiók közreműködői | Lehetővé teszi az intelligens rendszerfiókok kezelését, az azokhoz való hozzáférés nélkül. | Igen | 
Key Vault közreműködő | Lehetővé teszi a kulcstartók kezelését, de azokhoz való hozzáférés nélkül. | Igen | 
Tesztkörnyezet létrehozója | Lehetővé teszi a felügyelt Labs Azure Lab-fiókokban való létrehozását, kezelését és törlését. | Igen | 
Log Analytics közreműködő | Log Analytics közreműködő képes olvasni az összes figyelési és szerkesztési beállítást. A figyelési beállítások szerkesztése magában foglalja a virtuálisgép-bővítmény virtuális gépekhez való hozzáadását. a Storage-fiók kulcsainak beolvasása az Azure Storage-ból származó naplók gyűjtésének konfigurálásához; Automation-fiókok létrehozása és konfigurálása; megoldások hozzáadása; és az Azure Diagnostics konfigurálása az összes Azure-erőforráshoz. | Igen | 
Log Analytics olvasó | Log Analytics olvasó megtekintheti és megkeresheti az összes figyelési adatait, valamint megtekintheti a figyelési beállításokat, beleértve az Azure Diagnostics konfigurációjának megtekintését az összes Azure-erőforráson. | Nem | 
Logikai alkalmazás közreműködői | Lehetővé teszi a logikai alkalmazások kezelését, de nem változtatja meg a hozzájuk való hozzáférést. | Igen | 
Logic app-operátor | Lehetővé teszi a logikai alkalmazások olvasását, engedélyezését és letiltását, de nem szerkesztheti és nem frissíti őket. | Igen | 
Felügyelt alkalmazás operátori szerepköre | Lehetővé teszi műveletek olvasását és végrehajtását a felügyelt alkalmazás erőforrásain | Igen | 
Felügyelt alkalmazások olvasója | Lehetővé teszi az erőforrások olvasását egy felügyelt alkalmazásban, valamint a JIT-hozzáférés kérését. | Nem | 
Felügyelt identitás közreműködői | Felhasználóhoz rendelt identitás létrehozása, olvasása, frissítése és törlése | Igen | 
Felügyelt identitás operátora | Felhasználóhoz rendelt identitás olvasása és hozzárendelése | Igen | 
Felügyeleti csoport közreműködője | Felügyeleti csoport közreműködői szerepköre | Igen | 
Felügyeleti csoport olvasója | Felügyeleti csoport olvasójának szerepköre | Nem | 
Közreműködő figyelése | Beolvashatja az összes figyelési és a figyelési beállításokat. Lásd még: Ismerkedés a szerepkörökkel, az engedélyekkel és a biztonsággal a Azure Monitor. | Igen | 
Figyelési metrikák közzétevője | Lehetővé teszi az Azure-erőforrásokhoz való közzétételi mérőszámok közzétételét | Igen | 
Figyelő olvasó | Az összes figyelési adat (mérőszámok, naplók stb.) olvasása. Lásd még: Ismerkedés a szerepkörökkel, az engedélyekkel és a biztonsággal a Azure Monitor. | Nem | 
Hálózati közreműködő | Lehetővé teszi a hálózatok kezelését, az azokhoz való hozzáférés nélkül. | Igen | 
Új ereklye APM-fiók közreműködői | Lehetővé teszi New Relic Application Performance Management-fiókok és-alkalmazások kezelését, az azokhoz való hozzáférés nélkül. | Igen | 
Olvasó és adathozzáférés | Lehetővé teszi az összes megtekintését, de nem engedélyezheti a Storage-fiók vagy a tárolt erőforrás törlését vagy létrehozását. Az olvasási/írási hozzáférést is lehetővé teszi a Storage-fiókban található összes, a Storage-fiók kulcsaihoz való hozzáférés útján. | Igen | 
Redis Cache közreműködő | Lehetővé teszi a Redis gyorsítótárak kezelését, de azokhoz való hozzáférés nélkül. | Igen | 
Erőforrás-házirend közreműködője (előzetes verzió) | Előnézet Visszatöltötte-felhasználóktól, az erőforrás-házirend létrehozásához/módosításához, támogatási jegy létrehozásához és az erőforrások/hierarchia olvasásához szükséges jogosultságokkal. | Igen | 
Ütemező – feladattípusok közreműködői | Lehetővé teszi a Scheduler-feladatok összegyűjtését, de nem fér hozzájuk. | Igen | 
Search Service közreműködő | Lehetővé teszi a keresési szolgáltatások kezelését, az azokhoz való hozzáférés nélkül. | Igen | 
Biztonsági rendszergazda | Csak Security Center esetén: megtekintheti a biztonsági házirendeket, megtekintheti a biztonsági állapotokat, biztonsági házirendeket szerkeszthet, megtekintheti a riasztásokat és a javaslatokat | Igen | 
Security Manager (örökölt) | Ez egy örökölt szerepkör. Használja helyette a biztonsági rendszergazdát | Igen | 
Biztonsági olvasó | Csak Security Center esetén: megtekintheti a javaslatokat és riasztásokat, megtekintheti a biztonsági házirendeket, megtekintheti a biztonsági állapotokat, de nem végezhet módosításokat | Nem | 
Site Recovery-közreműködő | Lehetővé teszi Site Recovery szolgáltatás felügyeletét, kivéve a tár létrehozását és a szerepkör-hozzárendelést | Igen | 
Site Recovery-operátor | Lehetővé teszi a feladatátvételt és a feladat-visszavételt, de nem hajt végre más Site Recovery felügyeleti műveleteket | Igen | 
Site Recovery-olvasó | Lehetővé teszi, hogy megtekintse Site Recovery állapotát, de ne végezzen más felügyeleti műveleteket | Nem | 
Térbeli horgonyok fiók közreműködője | Lehetővé teszi a térbeli horgonyok kezelését a fiókban, de nem törli őket | Igen | 
Térbeli horgonyok fiókjának tulajdonosa | Lehetővé teszi a fiókban lévő térbeli horgonyok kezelését, beleértve azok törlését is | Igen | 
Térbeli horgonyok fiókjának olvasója | Lehetővé teszi a fiókban található térbeli horgonyok tulajdonságainak megkeresését és beolvasását | Nem | 
SQL-adatbázis közreműködői | Lehetővé teszi az SQL-adatbázisok kezelését, de azokhoz való hozzáférés nélkül. Emellett nem kezelheti a biztonsággal kapcsolatos házirendeket vagy a szülő SQL-kiszolgálókat. | Igen | 
SQL felügyelt példány közreműködője | Lehetővé teszi az SQL felügyelt példányok és a szükséges hálózati konfiguráció kezelését, de mások számára nem biztosít hozzáférést. | Igen | 
SQL-biztonságkezelő | Lehetővé teszi az SQL-kiszolgálók és-adatbázisok biztonsággal kapcsolatos házirendjeinek kezelését, az azokhoz való hozzáférés nélkül. | Igen | 
SQL Server közreműködő | Lehetővé teszi az SQL-kiszolgálók és-adatbázisok kezelését, de azokhoz való hozzáférés nélkül, és nem a biztonsággal kapcsolatos házirendjeiket. | Igen | 
Tárfiók-közreműködő | Engedélyezi a Storage-fiókok kezelését. Hozzáférést biztosít a fiók kulcsaként, amely a megosztott kulcsos hitelesítésen keresztüli hozzáféréshez használható. | Igen | 
A Storage-fiók kulcs-kezelő szolgáltatásának szerepköre | Engedélyezi a Storage-fiók hozzáférési kulcsainak listázását és újragenerálását. | Igen | 
Storage-blobadatok közreműködője | Azure Storage-tárolók és-Blobok olvasása, írása és törlése. Ha meg szeretné tudni, hogy mely műveletek szükségesek egy adott adatművelethez, tekintse meg a blob-és üzenetsor-műveletek meghívására vonatkozó engedélyeket. | Igen | 
Storage-blobadatok tulajdonosa | Teljes hozzáférést biztosít az Azure Storage blob-tárolók és-adatkészletekhez, beleértve a POSIX hozzáférés-vezérlés hozzárendelését. Ha meg szeretné tudni, hogy mely műveletek szükségesek egy adott adatművelethez, tekintse meg a blob-és üzenetsor-műveletek meghívására vonatkozó engedélyeket. | Igen | 
Storage-blobadatok olvasója | Azure Storage-tárolók és-Blobok olvasása és listázása. Ha meg szeretné tudni, hogy mely műveletek szükségesek egy adott adatművelethez, tekintse meg a blob-és üzenetsor-műveletek meghívására vonatkozó engedélyeket. | Nem | 
Storage blob-delegáló | Felhasználói delegálási kulcs beszerzése, amely az Azure AD-beli hitelesítő adatokkal aláírt tárolók vagy Blobok közös hozzáférési aláírásának létrehozásához használható. További információt a felhasználói delegálási SAS létrehozása című témakörben talál. | Igen | 
Storage-fájladatok SMB-megosztásának közreműködője | Lehetővé teszi az olvasási, írási és törlési hozzáférést az Azure Storage-fájlmegosztás SMB-en keresztül | Igen | 
Storage-fájladatok SMB-megosztásának emelt szintű közreműködője | Olvasási, írási, törlési és módosítási engedélyek engedélyezése az Azure Storage-fájlmegosztás SMB-kapcsolaton keresztüli eléréséhez | Igen | 
Storage-fájladatok SMB-megosztásának olvasója | Olvasási hozzáférés engedélyezése az Azure-fájlmegosztás SMB használatával | Nem | 
Tárolási várólista adatközreműködői | Azure Storage-várólisták és üzenetsor-üzenetek olvasása, írása és törlése. Ha meg szeretné tudni, hogy mely műveletek szükségesek egy adott adatművelethez, tekintse meg a blob-és üzenetsor-műveletek meghívására vonatkozó engedélyeket. | Igen | 
Tárolási üzenetsor adatüzenet-processzora | Üzenet betekintése, beolvasása és törlése egy Azure Storage-várólistából. Ha meg szeretné tudni, hogy mely műveletek szükségesek egy adott adatművelethez, tekintse meg a blob-és üzenetsor-műveletek meghívására vonatkozó engedélyeket. | Igen | 
Tárolási várólista adatüzenetének küldője | Üzenetek hozzáadása egy Azure Storage-várólistához. Ha meg szeretné tudni, hogy mely műveletek szükségesek egy adott adatművelethez, tekintse meg a blob-és üzenetsor-műveletek meghívására vonatkozó engedélyeket. | Igen | 
Storage-várólista adatolvasója | Azure Storage-várólisták és üzenetsor-üzenetek olvasása és listázása. Ha meg szeretné tudni, hogy mely műveletek szükségesek egy adott adatművelethez, tekintse meg a blob-és üzenetsor-műveletek meghívására vonatkozó engedélyeket. | Nem | 
Támogatási kérelem közreműködői | Lehetővé teszi a támogatási kérések létrehozását és kezelését | Igen | 
Traffic Manager közreműködő | Lehetővé teszi a Traffic Manager-profilok kezelését, de nem teszi lehetővé az azokhoz való hozzáférés szabályozását. | Igen | 
Felhasználói hozzáférés rendszergazdája | Lehetővé teszi az Azure-erőforrásokhoz való felhasználói hozzáférés kezelését. | Igen | 
Virtuális gép rendszergazdai bejelentkezése | Virtual Machines megtekintése a Portálon és Bejelentkezés rendszergazdaként | Igen | 
Virtuális gépek közreműködője | Lehetővé teszi a virtuális gépek kezelését, de nem fér hozzájuk, nem pedig a virtuális hálózati vagy a Storage-fiókhoz, amelyhez csatlakoznak. | Igen | 
Virtuális gép felhasználói bejelentkezés | Tekintse meg Virtual Machines a portálon, és jelentkezzen be normál felhasználóként. | Igen | 
Webes csomag közreműködői | Lehetővé teszi a webhelyek webes csomagjainak kezelését, de azokhoz való hozzáférés nélkül. | Igen | 
Webhely közreműködői | Lehetővé teszi a webhelyek (nem webes csomagok) kezelését, de nem fér hozzájuk | Igen |

## <a name="next-steps"></a>Következő lépések

- [Partner által szerzett kredit – áttekintés arról, hogyan működik a CSP új kereskedelmi felületén](partner-earned-credit.md)
