## Voice Agent Cost Lab

* Standalone browser calculator with **South India / USD / pay-as-you-go** model-price references.
* Compare managed Voice Agent / Voice Live tiers and **bring your own model (BYOM)** using list-price estimates.
* BYOM models and GPT Live use **South India Global** prices from Azure OpenAI.
* **Azure HD voice uses Central India rates** as requested.
* No South India Voice Live tier or BYO speech meters were found, so managed tiers and BYO STT also use the approved, explicitly labeled **Central India references**.

### Run

* With Node.js 20 or later ``` node .\server.mjs ```
* Test ``` node --test .\calculator.test.mjs .\server.test.mjs ```

* Changes are in memory only

### Price basis

* `prices.json` is a **2026-10-22 snapshot**, not a live price feed, from the [Azure Retail Prices API](https://prices.azure.com/api/retail/prices).
*  It records original billing units, exact USD prices, meter IDs, filters, and effective dates where returned.

<img width="1267" height="848" alt="image" src="https://github.com/user-attachments/assets/5adde47d-391c-4016-9261-25b90c54ef08" />
