## **Game Mechanic Specification — *Crafterse \- Craft your own Universe***

## **1\) Combat & Core Control**

**Góc nhìn & camera**

* Isometric/diagonal; camera bám nhân vật, zoom cố định; rung màn nhẹ theo impact (tắt/bật trong Settings).

**Điều khiển**

* **Di chuyển:** WASD / joystick.  
* **Ngắm/đánh:** chuột / right stick định hướng. Đòn thường có **aim-assist nhẹ** với mục tiêu gần (±6–8°).  
* **Né/Dodge:** lăn/nhảy ngắn, **i-frame** 0.20–0.30s *(gợi ý)*; **CD** 2.5–4.0s *(gợi ý, tuỳ build SPD)*.  
* **Kỹ năng chủ động:** 2 skill từ vũ khí; dùng **Năng lượng** (Energy) hoặc CD riêng.  
* **Tương tác:** F cho rương, shop, cột ban thưởng, NPC.

**Chỉ số cốt lõi**

* **ATK, DEF, HP, SPD, Crit Rate, Stamina/Energy, Slot.**  
* **Công thức gợi ý:**  
  * Sát thương thường \= ATK × (1 \+ Bonus%) × (1 − Giảm sát thương mục tiêu).  
  * Crit \= ×(1 \+ Crit Rate); Armor Break của **Kim** áp dụng trước giảm sát thương.  
* **Stamina/Energy:** tiêu hao cho dodge/skill; hồi theo thời gian; đồ/đá có thể tăng regen.

**Triết lý combat**

* Nhịp độ nhanh, “đòn thường → hiệu ứng on-hit → mở góc dùng skill → reposition”.  
* Khen thưởng **timing/định vị**; trừng phạt tham lam (dodge sai nhịp, đứng trong trap).

## **2\) NPC Mechanic (hệ thống gắn với NPC)**

**Elyssia – Dreamweaver**

* **Scroll System \= AI Prompt-to-Generate:** Prompt \+ **Scroll** (D→S) \+ **Scrap** → **Artifact Prompt**.  
* Lớp **validation/balancing** trước khi ra vật phẩm (lọc visual/lore, khung stat an toàn).

**Grimm – Forge Master**

* **Nâng cấp Guardian** bằng AC: HP/ATK/DEF/SPD. Không áp dụng trong PvP normalize.

**Zephyr – Merchant**

* Bán **trang bị/vũ khí khởi đầu**.

**Valorheart – Captain**

* Cửa vào **PvP Arena**; quản lý mode, xếp hạng, thưởng mùa.

**Boros – Elemental Smith**

* **Rèn**: Linh khí → **Đá nguyên tố** (rank D→S).  
* **Khảm/Rã đá** trên vũ khí; **phí rã** nhỏ (AC) để chống spam.  
* **Rã vũ khí** → trả **Scrap** \+ Essence/Linh khí/Rune Fragment (tuỳ loại).  
* **Swap skin vũ khí**: đổi ngoại hình, giữ nguyên stat/skill.

## **3\) Weapon Mechanic**

**Phân loại**

* **Artifact Prompt (nguời chơi tạo)** – Elyssia chế tác.  
* **Artifact Game (hệ thống cấp/bán)** – bảo đảm người chơi luôn có build nền.  
* **Weapon in-run** – chỉ tồn tại trong run; rời dungeon là mất.

**Bậc & socket**

* **D:** 0 nguyên tố, **3 socket**, **100 Scrap**.  
* **C:** 1–2 nguyên tố, **4 socket**, **150 Scrap**.  
* **B:** 2 nguyên tố, **6 socket**, **200 Scrap**.  
* **A:** 2–3 nguyên tố, **8 socket**, **300 Scrap**.  
* **S:** 3 nguyên tố, **10 socket**, **500 Scrap**.

**Thuộc tính vũ khí**

* **On-hit effect** (cố định theo nguyên tố chính; xem mục 5).  
* **2 kỹ năng chủ động** (hình thái/FX chịu ảnh hưởng prompt \+ nguyên tố).  
* **Socket**: khảm **Đá nguyên tố** để tăng **chỉ số bị động** (không cấp kỹ năng).

**Vòng đời**

* **Tạo → Dùng → Khảm/Rã đá → Rã vũ khí → Tái chế** (Scrap quay lại vòng lặp).  
* **Swap skin** tại Boros để “làm mới cảm giác” mà không phá cân bằng.

## **4\) Scroll System (AI Prompt-to-Generate)**

**Bậc Scroll**

* **D/C/B/A**: mua/cày; ảnh hưởng **khung stat** và **độ phức tạp skill**.  
* **S**: **chỉ craft** từ 3 nguyên liệu hiếm: **Heart of Ember, Frozen Tear, Ancient Bark**.

**Prompt**

* Văn bản tự do (ngắn \= random thú vị; dài \= bám ý đồ).  
* Ảnh hưởng **chủng vũ khí** (kiếm/cung/gậy/…); **FX/lore**; **đề xuất** bộ skill tương thích.

**Kết quả chịu ảnh hưởng bởi**

* Rank Scroll, **Scrap** sẵn có, **thành phần nguyên tố** mong muốn.  
* Lớp **validation** để vũ khí hợp gameplay (không phá game).

## **5\) Elemental & Stone Mechanic**

**Nguyên tố chính (5 hệ) & on-hit duy nhất**

* **Hỏa:** Burn (DOT; đủ stack → bùng nổ nhỏ).  
* **Thủy:** Freeze stack (làm chậm; đủ stack → Đóng Băng ngắn).  
* **Mộc:** Root/Slow ngắn (kiểm soát vị trí).  
* **Kim:** Armor Break (giảm DEF tạm thời).  
* **Thổ:** Stagger (tăng thanh choáng; đủ ngưỡng → Choáng ngắn).

**Đá nguyên tố (do Boros rèn)**

* **Nguồn:** quái rơi **Linh khí** theo hệ → rèn **Đá nguyên tố** (mặc định **10 Linh khí \= 1 Đá**).  
* **Rank D→S:** rank càng cao → **chỉ số bị động** mạnh hơn (ATK/DEF/HP/SPD/Crit/regen/kháng…).  
* **Khảm/rã tự do** (mất phí rã nhỏ bằng AC).  
* **Lưu ý:** Đá **không cấp kỹ năng**; chỉ bổ sung **passive** và **điểm nguyên tố** cho **Resonance**.

**Resonance (cộng hưởng bị động)**

* Tổng **điểm nguyên tố** từ **vũ khí \+ trang bị \+ đá** → kích các **mốc** (ví dụ **2/4/6/8**).  
* Mỗi hệ có **bộ hiệu ứng riêng** (ví dụ: Hỏa tăng dmg lên mục tiêu đang Burn; Kim hồi năng lượng khi hạ địch đang Armor Break…).  
* Có thể kích **nhiều hệ đồng thời** nếu đủ điểm.

## **6\) Dungeon Mechanic (PvE)**

**Cấu trúc run**

* **Map 1–4:** quái nhỏ/quái trung, trap room (khóa cửa), **rương**, **shop** (1–2 lần/map, tiêu **RC**), **cột ban thưởng** sau trap lớn.  
* **Map 5:** **Mini Boss** (đấu trường riêng).  
* **Boss chính:** mở sau mini boss (theo nhánh/act).  
* **Phần thưởng:** **Scrap**, **Linh khí**, **Đá nguyên tố**, **nguyên liệu hiếm** (craft Scroll S), **Ngọc nguyên tố** (tiến trình cốt truyện).

**RC – dungeon coin**

* Thu: quái, rương, event;  
* Dùng: shop/cột trong run;  
* **Reset** khi rời dungeon.

**Độ khó & nhịp**

* Tăng dần qua map; affix ngẫu nhiên (quái thêm kháng, trap dày hơn…).  
* Mục tiêu: luôn tạo “bài toán build” khác mỗi run.

## **7\) PvP Arena Mechanic**

**Loadout**

* Dùng **Artifact \+ trang bị** người chơi sở hữu (đã build sẵn).

**Normalize (công bằng)**

* Quy về **baseline stat** theo hạng; giữ **hành vi kỹ năng** & **on-hit** nhưng **scale sát thương/CC** về chuẩn.  
* Trang bị/đá chỉ **ảnh hưởng nhẹ**.

**Mode**

* **Battle Royale**.

## **8\) Progression Mechanic**

**Guardian (ngoài PvP)**

* **Grimm** tăng HP/ATK/DEF/SPD; tiêu **AC**.

**Artifact**

* **Craft** (Elyssia), **khảm đá** (Boros), **swap skin** (Boros), **nâng cấp nhẹ** qua nguyên liệu hiếm (không thay trần sức mạnh).

**Meta-progression sau run**

* **Thành công:** giữ toàn bộ tài nguyên.  
* **Thất bại:** mất **50%** tài nguyên.  
* **Thoát sớm:** mất **25%**.  
* Mục tiêu: luôn có tiến triển, nhưng vẫn “đau” để kích thích kỹ năng & build.

## **9\) Marketplace Mechanic**

**Web2 – Metadata / Lazy mint (cơ chế chờ)**

* **Tất cả item** (vũ khí, đá, scroll, nguyên liệu…) đều **trade được** ở trạng thái **metadata** (off-chain).  
* **Lazy mint** \= **chưa mint NFT** ngay; item di chuyển **trong hệ thống game**; chỉ khi người chơi muốn **đưa on-chain** mới mint thật.

**Web3 – NFT**

* Người chơi dùng **Mint Key** để **mint** item thành **NFT** trên blockchain.  
* NFT giao dịch được **cả in-game lẫn marketplace on-chain**.  
* **Custodial wallet**: mọi Web2 user đều có **ví ảo** (tạo tự động); có thể chuyển sang **ví thật** khi sẵn sàng.

**Phí & an toàn**

* **AC fee %** cho mỗi giao dịch (sink kinh tế).  
* Bộ **chống lạm dụng**: giới hạn số lần list, giá sàn mềm, phát hiện vòng giao dịch bất thường.  
* Truyền thông rõ: **NFT là tuỳ chọn**; gameplay cân bằng với **PvP normalize**.

## **10\) Economy Mechanic**

### **1\. Hệ tiền tệ (Currency System)**

* **RC (Run Coin):**  
  * Chỉ tồn tại trong Dungeon run.  
  * Thu từ: giết quái, mở rương, trap event.  
  * Dùng trong run: shop ngẫu nhiên, nâng cấp vũ khí, buff trụ.  
  * Reset khi rời dungeon (không mang ra ngoài).  
  * Vai trò: giữ **roguelite feel** – mỗi run là mới, không tích lũy RC để phá game.  
* **AC (Arcane Crystal):**  
  * Tiền tệ chính ở Hub/Marketplace.  
  * Nguồn: nạp tiền (pay) hoặc cày (play → đổi từ loot/tài nguyên).  
  * Dùng cho:  
    * Nâng cấp Guardian (Grimm).  
    * Mua scroll cơ bản/ trung/ nâng cao.  
    * Phí giao dịch Marketplace.  
    * Khảm/rã đá (Boros).  
    * Cosmetic shop.  
  * AC chia làm 2 nguồn:  
    * **AC nạp** (premium).  
    * **AC cày** (earnable).  
  * Cả 2 loại AC dùng chung trong giao dịch, nhưng **premium có ưu đãi** (ví dụ giảm phí trade, thêm slot bán).

### **2\. Nguyên liệu Craft & Loop tài nguyên**

* **Scrap (Mảnh sắt vụn):**  
  * Thu được khi rã vũ khí rác/dư.  
  * Dùng để craft Artifact mới (cần cùng với Scroll).  
  * Giữ vai trò “vòng lặp tuần hoàn” → không lãng phí item.  
* **Linh khí (Essence):**  
  * Rơi từ quái theo nguyên tố.  
  * Boros dùng để đúc thành **Đá nguyên tố**.  
* **Đá nguyên tố (Elemental Stone):**  
  * Rank D→S.  
  * Khảm vào socket vũ khí để tăng chỉ số bị động \+ điểm resonance.  
  * Có thể tháo/rã, trade trên Marketplace.

* **Nguyên liệu hiếm (Rare Materials):**  
  * Ví dụ: **Heart of Ember, Frozen Tear, Ancient Bark**.  
  * Chỉ rơi từ boss/mini-boss hoặc event đặc biệt.  
  * Bắt buộc để craft **Scroll S**.  
  * Sink quan trọng, giữ giá trị cho Dungeon farming.

### **3\. Scroll System (Weapon Prompt Economy)**

* **Scroll D→A:** bán ở Zephyr bằng AC.  
* **Scroll S:** chỉ craft từ nguyên liệu hiếm (khó farm), có giá trị cao.  
* Người chơi cần **Scrap \+ Scroll \+ Prompt \+ Đá nguyên tố** để Elyssia tạo Artifact.  
* Marketplace cho phép trade **Scroll hiếm** → tạo nhu cầu lớn.

### **4\. Marketplace Economy**

* **Web2 (Metadata Trading – Lazy Mint):**  
  * Người chơi có thể trade tất cả item (vũ khí, đá, scroll, nguyên liệu).  
  * Lazy mint: vật phẩm chỉ tồn tại trong hệ thống game (off-chain).  
  * Ưu điểm: nhanh, không phí gas, dễ tiếp cận free-player.  
* **Web3 (NFT Trading):**  
  * Dùng **Mint Key** để biến item thành NFT on-chain.  
  * NFT trade được cả in-game lẫn trên blockchain marketplace.  
  * Tích hợp custodial wallet cho Web2 player (ví ảo → rút ra ví thật khi muốn).  
* **Fee Structure:**  
  * 5–10% phí giao dịch (bằng AC).  
  * Premium user có thể được giảm phí hoặc tăng slot bán.  
  * Doanh thu chính: phí trade \+ IAP cosmetic.

### **5\. Economy Sink (ngăn lạm phát)**

Các điểm tiêu AC/nguyên liệu chính:

* **Nâng cấp Guardian** (Grimm).  
* **Craft Scroll S** (nguyên liệu hiếm \+ Rune Fragment).  
* **Khảm / rã đá** (Boros, có phí AC).  
* **Phí giao dịch marketplace** (AC fee).  
* **Cosmetic shop** (skin, effect, pet).  
* **Founder Pack / Event item** (IAP).

→ Đảm bảo mọi nguồn tài nguyên đều có sink → không bị “overflow”.

### **6\. Web2 ↔ Web3 Bridge**

* Web2 player trade bằng metadata (AC fee).  
* Khi muốn mint NFT: cần **Mint Key** \+ phí gas.  
* Có thể áp dụng **batch mint** hoặc **gasless quota** để giảm phí.  
* Kiểm soát AML (anti money laundering): KYC nhẹ khi rút NFT ra on-chain, hạn chế spam trade.

### **7\. Income Streams (Publisher)**

* **Phase 2 (MVP):** chưa tập trung doanh thu → tập trung tăng user.

* **Phase 3:**  
  * IAP cosmetic (skin, pet, effect).  
  * Founder Pack.  
  * Marketplace trade fee.  
* **Phase 4:**  
  * UGC Marketplace (map, quest, pet).  
  * Collab IP skin/vũ khí.  
  * Premium Subscription (extra prompt slot, giảm fee).  
  * Esport sponsorship.