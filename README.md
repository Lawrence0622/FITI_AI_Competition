這份報告的重點是介紹一個智慧跌倒偵測系統的設計理念、軟硬體架構、成果展示以及未來展望。
報告中強調了跌倒對老年人的危害，並指出傳統解決方案（如監視器和穿戴式裝置）的不足之處。
以下是該系統的主要特色：

●  軟體方面:
  ○  採用 human_detection_model 作為預訓練模型進行自有資料集的fine-tune，並針對 VA8801 開發板進行了轉檔和量化處理。
  ○  設計演算法結合line notify API，讀取模型輸出log，判定訊息發送，達到跌倒偵測系統功能。
  ○  模型的準確率為 90.5%，召回率為 76.3%。

●  硬體方面:
  ○  使用 VA8801 開發板作為運算核心，具有高效能、低功耗的優點。
  ○  外殼採用 PLA 塑膠 3D 列印，具有環保、可回收、易於設計和修改的特性。

●  實際應用:
  ○  系統可單獨使用於私人空間，例如浴室或臥室，因為沒有雲端資料庫儲存功能，無隱私疑慮。
  ○  也可以與傳統監視器搭配使用，以較低成本覆蓋更大範圍，適用於醫院或養老院等場所。

未來展望:

●  開發團隊希望將系統應用於更廣泛的領域，例如農作物監測、水質污染監測、海洋資源監測和森林盜伐預防。
●  未來改進方向包括軟體方面部署更新、更高效能的 YOLO 模型，以及硬體方面使用更耐用的材質和整合更多功能模組，像是串連LLM達到更豐富的語言互動。

----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

This report introduces the design concept, hardware and software architecture, results demonstration, and future outlook of an intelligent fall detection system.
The report emphasizes the dangers of falls to the elderly and points out the limitations of traditional solutions (such as surveillance cameras and wearable devices).
Key features of the system:

●  Software Aspects:
  ○  Uses a human_detection_model as a pre-trained model for fine-tuning with our own dataset, with file conversion and quantization processing specifically for the VA8801 development board.
  ○  Designed an algorithm that integrates with the Line Notify API, reads model output logs, determines message sending, achieving fall detection system functionality.
  ○  The model achieves 90.5% accuracy and 76.3% recall rate.

●  Hardware Aspects:
  ○  Uses the VA8801 development board as the computing core, featuring high performance and low power consumption.
  ○  The casing is 3D printed using PLA plastic, which is environmentally friendly, recyclable, and easy to design and modify.

●  Practical Applications:
  ○  The system can be used independently in private spaces such as bathrooms or bedrooms, with no privacy concerns due to the absence of cloud database storage.
  ○  It can also be integrated with traditional surveillance systems to cover larger areas at lower costs, suitable for hospitals or nursing homes.

Future Prospects:

●  The development team hopes to expand the system's applications to broader fields, such as:
-Crop monitoring
-Water pollution monitoring
-Marine resource monitoring
-Forest logging prevention

●  Future improvements include:
-Software deployment updates
-More efficient YOLO models
-Hardware upgrades with more durable materials
-Integration of additional functional modules, such as connecting with LLMs for richer language interaction
