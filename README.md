# RFID‑Based Smart Trolley with Automatic Billing

**Motive**  
Reduce supermarket checkout queues by moving item scanning and bill generation into the trolley itself, so customers see and manage their running bill in real time while they shop.

**System & Hardware**  
- Arduino‑based trolley with an RFID reader that scans tagged products as they are added or removed. [web:31][web:33][web:36][web:37]  
- 16×2 I2C LCD (or touch display in future), red/green LEDs, and a buzzer give immediate feedback for each scan and show the current total. [web:31][web:33][web:35]  

**What I did**  
- Implemented serial‑based RFID tag reading logic to capture each product’s unique ID and mapped those IDs to specific items (biscuits, chocolate, chips, ice cream, etc.) and prices. 
- Built an **automatic billing engine** on the microcontroller that increments or decrements the total in real time as tags are scanned, with separate flows for adding and deleting items.  
- Integrated user feedback: the LCD shows item name and price, LEDs and buzzer confirm successful scans, and a final tag press prints the total bill with a “thank you” message.
- 
**Explanation / Outcome**  
Together, the RFID reader, LCD interface, and billing logic form a **smart trolley** that continuously tracks items and cost inside the cart, so customers can finish payment directly from the trolley instead of waiting at a traditional checkout counter, making the in‑store experience faster and more transparent. 
