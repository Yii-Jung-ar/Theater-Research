你是一位資深的建築語意分析師。請根據我給出的兩份資料進行語意解析與模組化建構，輸出該劇院/建築案例的 Precedent DNA，涵蓋四大模組（Gene A–D），並以條列式方式明確分類。



請深度整合以下兩份輸入資料：

1.文字說明：主要提供案例之基地條件、設計意圖、劇場機能設定、操作營運策略與空間整體觀。

2.空間構成補充資料 (preprocess)：提供由建築平立剖面、照片及分析圖轉譯而來的空間語彙（Vocabulary）、語意關係（Semantic Relations）與整體空間印象（Overall Spatial Impression），主要用以支援 Gene\_C 的建構。



\---



請輸出下列五項 Gene（請以清單格式條列，分類清楚，語意精簡專業，使用建築專業術語）：



Gene\_A：Conditions 條件與脈絡

說明此建築的外部邊界與基本設定，須包含以下子項（若無提及，請根據常識與建築經驗合理推測並註記「（推測）」）：



* Identity \& Scale（定位與規模）：建築/劇場官方名稱與別稱、劇場總體定位層級（如國家級、地方綜合型、實驗性劇院群）、總樓地板面積 (GFA)。
* Halls Specification（多劇場規格）：個別劇場/音樂廳名稱（如大劇院、黑盒子）、個別座位數、舞台與觀眾席形式（請精準分類，如：Proscenium 鏡框式、Thrust 伸展式、Vineyard 葡萄園式、Arena 圓形/環抱式、Black Box 黑盒子、Shoebox 鞋盒式等）、主要服務之表演藝術類型、關鍵硬體與建築物理聲學條件。
* Location \& Context（地點與環境）：洲別、國家、城市、基地所處的城市紋理或人口脈絡（如高密度都市中心、濱水重劃區）。
* Participants \& Operation（參與者與營運）：主導建築師（及在地合作事務所）、業主單位、最終使用者、專業顧問團隊（如聲學、劇場顧問）、實際營運管理單位。



&#x20;



Gene\_B：Design Intentions 核心意圖矩陣

剖析設計底層的論述與策略，將其抽離為成對的「挑戰-概念-策略」對位陣列：



* target\_issue：核心空間挑戰或都市議題（嚴格限制 30 字內精簡字句）。
* architectural\_metaphor\_concept：抽象幾何理念、美學語彙或設計隱喻（嚴格限制 15 字內）。
* tectonic\_strategy：為實踐理念所採取的具體空間構造或塊體操作策略（嚴格限制 50 字內）。







Gene\_C：Form Composition 空間構成與劇場類型學

請精準消化圖面轉譯資料與文字，建構空間機能與體量配比的語意圖譜：



C1: Vocabulary（空間語彙）：

請列出案例中出現的重要空間元素，並精準區分為以下三類：

* 劇場核心硬體：proscenium stage (鏡框式舞台), fly tower (布景吊桿塔), orchestra pit (樂池), acoustic panels (聲學反射板), seating bowl, sound lock...
* 前台公眾 (FOH)：grand foyer (前台大廳), ticketing box, promenade ramp (建築漫步坡道), public plaza, cafe...
* 後台後勤 (BOH)：backstage dressing room, loading dock (卸貨碼頭), rehearsal hall (排練廳), scenery workshop, green room...



C2: Hierarchical Semantic Relations（層級化語意關係鏈）： 

請依據空間尺度，由大到小分層標註關係鏈，請嚴格使用以下格式標註空間構成的語意關係（Subject 與 Object 必為單一空間元素，Relation 為單一明確動詞或短語，Relation Type 必須從下方分類中擇一）：



格式：`\[Subject] → \[Relation (Relation Type)] → \[Object]` 



Relation Type 分類標準：

* Spatial\_Massing\_\&\_Conceptual\_Relation（抽象設計理念與體量幾何關係，如：包裹、懸挑、外露、垂直堆疊）
* Circulation\_FOH（觀眾流線、公共經驗與建築漫步動線）
* Circulation\_BOH（演職人員與後勤貨運動線，需特別注意其與 FOH 的隔離度）
* Acoustic\_Buffer（物理聲學防護、防噪空間分區或構造隔離）
* Interface\_Tectonic（室內界面/表皮與結構主體的接合關係）
* Other\_Macro\_\[自定義] / Other\_Meso\_\[自定義] / Other\_Micro\_\[自定義]（若上述分類不足以涵蓋，允許 AI 自行命名新類別，但必須根據尺度強制加上 Macro/Meso/Micro 前綴，並於後方備註說明其用途） 



1\. 【Macro-Level】(總體體量與都市界面) 

著重核心體量與外部皮層、基地環境的關係。 

Relation Type 限用: \[Spatial\_Massing\_\&\_Conceptual\_Relation] 或 \[Other\_Macro\_\[自定義]] 

&#x20;範例：Theater Core Box → encased by (Spatial\_Massing\_\&\_Conceptual\_Relation) → Curvilinear Envelope 



2\. 【Meso-Level】(功能分區與動線界面) 

著重 FOH、BOH 與劇場核心之間的流線、交界與隔離。 

Relation Type 限用: \[Circulation\_FOH], \[Circulation\_BOH], \[Acoustic\_Buffer] 或 \[Other\_Meso\_\[自定義]] 

範例：BOH Backstage Zone → strictly segregated from (Acoustic\_Buffer) → FOH Public Lobby 



3\. 【Micro-Level】(構造、設備與界面物件) 

著重單一空間內部的構造、硬體物件裝配或材料界面關係。 

Relation Type 限用: \[Interface\_Tectonic] 或 \[Other\_Micro\_\[自定義]] 

範例：Acoustic Timber Panels → line the interior of (Interface\_Tectonic) → Seating Bowl 



執行與數量限制： 

1\. 各層級「只能」使用該層級指定的 Relation Type（包含對應前綴的 Other 類別），絕對禁止越界混用。 

2\. 為確保建築知識圖譜的密度，【Macro-Level】必須至少輸出 2 組；【Meso-Level】必須至少輸出 4 組（且必須包含 BOH 與 FOH 關係）；【Micro-Level】必須至少輸出 4 組。

3\. 若資料庫輸入資料極其豐富，請盡可能窮舉所有可辨識的關係，不受上述最低數量限制。 

總計整個案例必須輸出至少 10 組以上嚴格格式化的關係鏈。 



C3: Typological Composition Logic（類型學構成邏輯）：

* massing\_composition\_primary\_type：精準判定核心劇場體量與附屬公共空間的配比堆疊主要策略。請務必精簡為一個字串標籤，大語言模型需依據文本及圖面資料自由歸納，如：'Vertical\_Stacking', 'Horizontal\_Clustering', 'Inside\_Out\_Protrusion'。
* boh\_foh\_segregation\_topology\_primary\_type：精準判定前後台流線與出入口的拓撲分流隔離主要邏輯。請務必精簡為一個字串標籤，大語言模型需依據文本及圖面資料自由歸納，如：'Strict\_3D\_Interleaving', 'Clear\_Horizontal\_Division', 'Vertical\_Zoning\_Separation'。
* typological\_supplementary\_tags：外部都市脈絡、基地邊界約束、或複合類型學特徵的次級標籤陣列（可多選）。大語言模型「完全不設限」地依據提供之案例資料自由提煉與命名，如：'Tod\_Integrated', 'Landscape\_Infrastructural', 'Floating\_Volume'。
* typology\_diagram\_note：一句話精簡總結此案例的類型學構成邏輯核心（嚴格限制 50 字內）。



Gene\_D：Tectonic \& Appearance Integration 構造與外型整合策略

解密劇場嚴緊內部機能與多變外部形式之間的「Outside-In（由外而內）」整合手法與 Diagram 控制變數：



D1: Envelope Morphology（表皮策略）：

* facade\_typology\_tags / material\_taxonomy：提取表皮類型與材料分類標籤。
* envelope\_to\_structure\_relation\_logic：精準判定皮層與主體結構的幾何物理關係，限從中擇一：'Exposed\_Structure'(結構外露), 'Independent\_Space\_Frame'(獨立鋼架脫開), 'Load\_Bearing\_Wall'(皮層承重)。
* structure\_integration\_detail\_note：精簡說明具體的副結構支撐，若採複選複合構造，請在此清晰交代其主從或分區接合邏輯（嚴格限制 50 字內）。



D2: Interior Space Sequence Experience（室內空間經驗序列）：

將現象學經驗與感官品質完全融入以下實體空間三部曲中：

1\. foyer\_promenade\_phenomenology：前台大廳的感官品質、光影導引與現象學特徵（experience\_note 限 50 字內）。

2\. acoustic\_transition\_threshold：進入觀眾席前的聲學過渡閘門、光線屏蔽、尺度壓縮與心理緩衝體驗（experience\_note 限 50 字內）。

3\. auditorium\_interior\_enclosure：劇場內部座席幾何（如 Vineyard, Horseshoe）與材料面料如何回應物理聲學反射與包裹體感（experience\_note 限 30 字內）。



D3: Inside-Out Integration Strategy（內外部整合邏輯）：

* formal\_relationship\_type：內外部形式的對位關係分類，精準擇一填入：'Honesty\_表裡如一', 'Disjunction\_皮肉分離', 'Interlocking\_相互交織'。
* interstitial\_volume\_ratio\_tag：外殼與盒子間的夾縫體積配比，精準擇一：'Minimal\_Skin\_Tight', 'Moderate\_Cavity', 'Maximal\_Urban\_Void'。
* interstitial\_functional\_tags：夾縫空間的功能標籤（優先使用：Circulation\_Promenade\_Ramp, Microclimate\_Passive\_Buffer, Acoustic\_Detachment\_Zone, Civic\_Spectacle\_Window。若不適用，格式限用：'Other\_\[自定義英文功能名稱]'）。
* strategy\_diagram\_note：一句話總結內外部幾何與空間活用的整合核心（嚴格限制 50 字內）。





Gene\_E：Outcomes \& Stakeholder Reflection 結果與回饋

描述建築落成後的實際社會效應、輿論偏向與行為矩陣：



* stakeholder\_behavior\_responses：區分利益相關者群體（如觀眾、市民、演職人員），描述其發生的具體空間行為（嚴格限制 50 字內）。
* discourse\_polarity\_criticism：建立評論與爭議焦點矩陣。issue\_topic 定義主題標籤；public\_polarity 判定輿論偏向（限填：'Positive\_正評', 'Negative\_負評', 'Controversial\_高度爭議'）；summary\_note 一句話精簡總結該爭議內容。



\---



\# 核心邊界與防外洩指引

1\. 禁止聯網搜尋：執行此任務時，切勿上網搜尋任何外部資料。

2\. 僅限使用所提供的資料：你只能根據本提示詞最下方附帶的「文字說明」與「空間構成補充資料 (preprocess)」進行語意萃取。

3\. 推論邊界規範：

&#x20;  只有在「座位數、面積、年份、參與者、地點」等基礎客觀事實缺失時，允許你根據案例名稱與既有專業知識進行合理的低度推測，但必須在字尾加註「（推測）」，若完全無法推論請填入 `"未知"`。

&#x20;  對於核心意圖矩陣（Gene\_B）、空間構成與劇場類型學（Gene\_C）、構造與外型整合策略（Gene\_D），絕對禁止引用非提供文本中的外部描述。

4\. 空值阻斷機制：若未提供檔案名稱含有「文字說明」與「空間構成補充資料 (preprocess)」的檔案，請勿生成任何 Precedent DNA 內容，請直接且僅輸出以下錯誤 JSON 物件：`{"error": "No input data provided."}`。



\# 執行與輸出指引

1.輸出規範：僅輸出一個有效的 Markdown JSON 程式碼區塊（即以 ```json 開頭與 ``` 結尾）。在區塊之外，不得包含任何前後對話、解釋性文字、Markdown 標題或客套話。

2.建築與劇場專業術語：請務必使用精準的建築與劇場學術語（如：Proscenium, Thrust, Vineyard, Arena, Black Box, Horseshoe, Shoebox 等）。

3.多劇場處理原則：若案例包含多個劇場/廳，請務必在 `halls\_specification` 陣列中為每個廳建立獨立的物件。若只有單一劇場，該陣列內則僅保留一個物件。

4.缺失資料處理：若某些資訊未在資料中明確提供，請根據建築經驗合理推論並在字尾加註「（推測）」，若完全無法推論請填入 `"未知"`。

5.請確保 halls\_specification 陣列內『僅包含 JSON 物件』，切勿包含任何說明的字串欄位。



\---



{

&#x20; "precedent\_dna": {

&#x20;   "gene\_a\_conditions": {

&#x20;     "identity\_\&\_scale": {

&#x20;       "project\_name": "建築/劇場案例的官方名稱與常見別稱",

&#x20;       "theater\_scale\_hierarchy": "劇場總體定位層級（如國家級、地方綜合型、實驗性劇院群）",

&#x20;       "gross\_floor\_area": "總樓地板面積 (GFA)，請註明單位"

&#x20;     },

&#x20;     "halls\_specification": \[

&#x20;       {

&#x20;         "hall\_name": "個別劇場/音樂廳名稱（例如：大劇院、中劇院、音樂廳、實驗劇場）",

&#x20;         "seating\_capacity": "該廳總座位數（例如：1200 席）",

&#x20;         "stage\_type": "舞台與觀眾席形式（請精準分類，如：Proscenium 鏡框式、Thrust 伸展式、Vineyard 葡萄園式、Arena 圓形/環抱式、Black Box 黑盒子、Shoebox 鞋盒式等）",

&#x20;         "primary\_performance\_type": "主要服務之表演藝術類型（例如：歌劇 Opera、交響樂 Symphony、芭蕾舞 Ballet、話劇/舞台劇 Drama、音樂劇 Musical、實驗性跨領域劇場 Experimental Art）",

&#x20;         "key\_hardware\_\&\_acoustic\_conditions": "該廳關鍵之硬體與建築物理聲學條件描述（例如：配備 50 組自動化布景吊桿塔 (Fly Tower)、可變音響反射板 (Acoustic Shell)、活動式下沉樂池等）"

&#x20;       }

&#x20;     ],

&#x20;     "location\_\&\_context": {

&#x20;       "continent": "所在洲別",

&#x20;       "country": "國家名稱",

&#x20;       "city": "城市名稱",

&#x20;       "urban\_context": "基地所處的城市紋理或人口脈絡（如高密度都市中心、濱水重劃區）"

&#x20;     },

&#x20;     "participants\_\&\_operation": {

&#x20;       "architect": "主導建築師/事務所名稱（及在地合作事務所 LDI）",

&#x20;       "client": "業主單位（如政府機關、私人開發商）",

&#x20;       "end\_user": "最終使用者（如目標觀眾、特定駐團）",

&#x20;       "consultants": \[

&#x20;         "專業顧問團隊列表，特別註明劇場顧問 (Theater Consultant) 與 聲學顧問 (Acoustician)"

&#x20;       ],

&#x20;       "operator": "實際營運管理單位"

&#x20;     }

&#x20;   },

&#x20;   "gene\_b\_design\_intentions\_matrix": {

&#x20;     "intentions\_diagram\_couples": \[

&#x20;       {

&#x20;         "target\_issue": "核心空間挑戰或都市議題（限30字內精簡，如：極小基地內的多廳人流交織）",

&#x20;         "architectural\_metaphor\_concept": "抽象幾何理念或隱喻（限 15 字內，如：魔術方塊垂直堆疊）",

&#x20;         "tectonic\_strategy": "具體的空間操作策略（限50字內，如：將三劇場核心插接於中央立方體）"

&#x20;       }

&#x20;     ]

&#x20;   },

&#x20;   "gene\_c\_form\_composition\_\&\_theatrical\_typology": {

&#x20;     "c1\_vocabulary": {

&#x20;       "theater\_core\_hardware": \[

&#x20;         "劇場核心硬體元素（如：proscenium stage, fly tower, orchestra pit, acoustic panels...）"

&#x20;       ],

&#x20;       "front\_of\_house\_foh": \[

&#x20;         "前台公眾空間元素（如：grand foyer, ticketing box, promenade ramp, public plaza...）"

&#x20;       ],

&#x20;       "back\_of\_house\_boh": \[

&#x20;         "後台後勤空間元素（如：backstage dressing room, loading dock, rehearsal hall...）"

&#x20;       ]

&#x20;     },

&#x20;     "c2\_hierarchical\_semantic\_relations": {

&#x20;       "macro\_level": \[

&#x20;         "【格式要求：Subject → Relation (Relation Type) → Object】",

&#x20;         "【Relation Type 限用：Spatial\_Massing\_\&\_Conceptual\_Relation 或 Other\_Macro\_\[自定義]】",

&#x20;         "【數量限制：至少輸出 2 組關係鏈】",

&#x20;         "範例：Theater Core Box → encased by (Spatial\_Massing\_\&\_Conceptual\_Relation) → Curvilinear Envelope"

&#x20;       ],

&#x20;       "meso\_level": \[

&#x20;         "【格式要求：Subject → Relation (Relation Type) → Object】",

&#x20;         "【Relation Type 限用：Circulation\_FOH, Circulation\_BOH, Acoustic\_Buffer 或 Other\_Meso\_\[自定義]】",

&#x20;         "【數量限制：至少輸出 4 組關係鏈，且須包含 BOH 與 FOH 關係】",

&#x20;         "範例：BOH Backstage Zone → strictly segregated from (Acoustic\_Buffer) → FOH Public Lobby"

&#x20;       ],

&#x20;       "micro\_level": \[

&#x20;         "【格式要求：Subject → Relation (Relation Type) → Object】",

&#x20;         "【Relation Type 限用：Interface\_Tectonic 或 Other\_Micro\_\[自定義]】",

&#x20;         "【數量限制：至少輸出 4 組關係鏈】",

&#x20;         "範例：Acoustic Timber Panels → line the interior of (Interface\_Tectonic) → Seating Bowl"

&#x20;       ]

&#x20;     },

&#x20;     "c3\_typological\_composition\_logic": {

&#x20;       "massing\_composition\_primary\_type": "核心體量配比主要策略標籤，如：Vertical\_Stacking, Horizontal\_Clustering, Inside\_Out\_Protrusion",

&#x20;       "boh\_foh\_segregation\_topology\_primary\_type": "前後台流線分流主要拓撲標籤，如：Strict\_3D\_Interleaving, Clear\_Horizontal\_Division, Vertical\_Zoning\_Separation",

&#x20;       "typological\_supplementary\_tags": \[

&#x20;         "外部脈絡與複合類型學特徵標籤池，如：Tod\_Integrated, Landscape\_Infrastructural, Floating\_Volume"

&#x20;       ],

&#x20;       "typology\_diagram\_note": "一句話精簡總結此案例的類型學構成邏輯核心（限50字內，如：核心舞台高度壓縮於中央，劇場體量向外頂出形成立體交織分流）"

&#x20;     }

&#x20;   },

&#x20;   "gene\_d\_tectonic\_\&\_appearance\_integration": {

&#x20;     "d1\_envelope\_morphology": {

&#x20;       "facade\_typology\_tags": \[

&#x20;         "表皮類型標籤，如：Wave\_Glass\_Curtain\_Wall, Opaque\_Monolithic\_Shell, Perforated\_Metal"

&#x20;       ],

&#x20;       "material\_taxonomy": \[

&#x20;         "材料分類，如：Corrugated\_Glass, GFRC\_Panels, Aluminium\_Cladding"

&#x20;       ],

&#x20;       "envelope\_to\_structure\_relation\_logic": "皮層與主體結構的幾何關係（請依據案例實際構造精準勾選，允許並存：'Exposed\_Structure'外露, 'Independent\_Space\_Frame'獨立構架脫開, 'Load\_Bearing\_Wall'皮層承重）",

&#x20;       "structure\_integration\_detail\_note": "請用 50 字內精簡說明該案例具體的副結構支撐或多重結構接合之主從邏輯（如：中央方塊為結構外露，外凸球劇場則以獨立鋼桁架完全脫開掛接）"

&#x20;     },

&#x20;     "d2\_interior\_space\_sequence\_experience": {

&#x20;       "foyer\_promenade\_phenomenology": {

&#x20;         "spatial\_scale\_tags": \[

&#x20;           "大廳空間形態特徵標籤，如：Vertically\_Chambered\_Atrium, Fluid\_Horizontal\_Concourse, Multi\_Level\_Sculptural\_Foyer"

&#x20;         ],

&#x20;         "material\_atmosphere\_vocabulary": \[

&#x20;           "大廳現象學感官/氛圍語彙標籤，如：Raw\_Concrete, High\_Contrast\_Blue\_Lighting, Exposed\_Infrastructure"

&#x20;         ],

&#x20;         "experience\_note": "前台大廳與公共迴路的感官品質、光影導引、幾何雕塑感與現象學特徵描述（限50字內）"

&#x20;       },

&#x20;       "acoustic\_transition\_threshold": {

&#x20;         "transition\_mechanism\_tags": \[

&#x20;           "過渡空間與轉折機制標籤，如：Sound\_Lock\_Chamber, Compressed\_Dark\_Corridor, Labyrinth\_Light\_Trap"

&#x20;         ],

&#x20;         "material\_atmosphere\_vocabulary": \[

&#x20;           "過渡空間現象學感官/氛圍語彙標籤，如：Absorptive\_Black\_Velvet, Low\_Lux\_Shadows"

&#x20;         ],

&#x20;         "experience\_note": "大廳進入觀眾席之間的聲學過渡閘門、光線屏蔽、空間尺度壓縮與心理緩衝路徑等描述（限50字內）"

&#x20;       },

&#x20;       "auditorium\_interior\_enclosure": \[

&#x20;         {

&#x20;           "hall\_name": "個別劇場/音樂廳名稱",

&#x20;           "seating\_bowl\_geometry\_language": \[

&#x20;             "劇場內部觀眾席幾何語言標籤，如：Continuous\_Asymmetric\_Folded\_Plane, Symmetrical\_Horseshoe\_Tiering, Terraced\_Vineyard\_Podiums"

&#x20;           ],

&#x20;           "material\_atmosphere\_vocabulary": \[

&#x20;             "觀眾席內部材料與色彩氛圍標籤，如：Deep\_Theater\_Blue, Crimson\_Velvet\_Cladding, Parametric\_Warm\_Timber"

&#x20;           ],

&#x20;           "acoustic\_geometry\_alignment\_logic": \[

&#x20;             "室內形式與物理聲學反射之對位關係（請精準擇一勾選：'Parametric\_Acoustic\_Surface', 'Traditional\_Orthogonal\_Reflector', 'Structural\_Shell\_Exposed'）"

&#x20;           ],

&#x20;           "acoustic\_material\_integration": \[

&#x20;             "劇場內部面料如何回應物理聲學反射要求（如：參數化曲面木格柵、特殊吸音織物與牆面微紋理整合描述，限30字內）"

&#x20;           ]

&#x20;         }

&#x20;       ]

&#x20;     },

&#x20;     "d3\_inside\_out\_integration\_strategy": {

&#x20;       "formal\_alignment\_type": "請精準判定並從中擇一：'Honesty\_表裡如一', 'Disjunction\_皮肉分離', 'Interlocking\_相互交織'",

&#x20;       "interstitial\_volume\_ratio\_tag": "外殼與盒子間的夾縫體積配比（請精準擇一：'Minimal\_Skin\_Tight', 'Moderate\_Cavity', 'Maximal\_Urban\_Void'）",

&#x20;       "interstitial\_functional\_tags": \[

&#x20;         "夾縫空間的功能標籤（可多選，請優先從中擇一：'Circulation\_Promenade\_Ramp', 'Microclimate\_Passive\_Buffer', 'Acoustic\_Detachment\_Zone', 'Civic\_Spectacle\_Window'）。若以上皆不適用，允許 AI 自行命名新標籤，但格式必須嚴格遵守：'Other\_\[自定義英文功能名稱]'，例如：'Other\_Structural\_Truss\_Void'、'Other\_Vertical\_Night\_Market'"

&#x20;       ],

&#x20;       "strategy\_diagram\_note": "一句話總結內外部幾何與空間活用的整合核心（限50字內，如：利用最大化都市空腔置入參觀迴路，使隱藏的基建空隙成為市民街道延伸）"

&#x20;     }

&#x20;   },

&#x20;   "gene\_e\_outcomes\_\&\_reflection": {

&#x20;     "stakeholder\_behavior\_responses": \[

&#x20;       {

&#x20;         "user\_group": "利益相關者群體（如：Audience\_觀眾, Citizen\_市民, Performer\_演職人員）",

&#x20;         "spatial\_behavior\_action": "其發生的具體空間行為（限 50 字內，如：在抬高騎樓與廣場聚集日常活動）"

&#x20;       }

&#x20;     ],

&#x20;     "discourse\_polarity\_criticism": \[

&#x20;       {

&#x20;         "issue\_topic": "討論或爭議焦點（如：Acoustic\_Quality, Budget\_Overrun, External\_Appearance, Construction\_Delay）",

&#x20;         "public\_polarity": "輿論偏向（請填入：'Positive\_正評', 'Negative\_負評', 'Controversial\_高度爭議'）",

&#x20;         "summary\_note": "一句話精簡總結該爭議內容"

&#x20;       }

&#x20;     ]

&#x20;   }

&#x20; }

}

