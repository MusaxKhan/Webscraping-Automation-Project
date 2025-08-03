# Webscraping-Automation-Project
𝗪𝗲𝗯 𝗦𝗰𝗿𝗮𝗽𝗶𝗻𝗴 𝗮𝗻𝗱 𝗔𝘂𝘁𝗼𝗺𝗮𝘁𝗶𝗼𝗻 𝗣𝗿𝗼𝗷𝗲𝗰𝘁: 𝗛𝗼𝘁𝗳𝗿𝗼𝗴 𝗕𝘂𝘀𝗶𝗻𝗲𝘀𝘀 𝗗𝗶𝗿𝗲𝗰𝘁𝗼𝗿𝘆

Recently worked on an automation project focused on extracting supplier company data from the https://www.hotfrog.com business directory. The goal was to collect relevant credentials of companies related to a specific search term and store them in a structured format for further use.



𝗣𝗿𝗼𝗯𝗹𝗲𝗺 𝗔𝗽𝗽𝗿𝗼𝗮𝗰𝗵

Hotfrog does not provide a public API for structured data, which made web scraping the most effective approach. However, the site dynamically loads some of its content, so a hybrid method combining both Selenium for navigation and BeautifulSoup for parsing static HTML was used. This ensured complete access to loaded content without losing performance or reliability.



𝗧𝗼𝗼𝗹𝘀 𝗮𝗻𝗱 𝗟𝗶𝗯𝗿𝗮𝗿𝗶𝗲𝘀

 • 𝗦𝗲𝗹𝗲𝗻𝗶𝘂𝗺 – For automated browser control and handling dynamic content rendered via JavaScript.

 • 𝗕𝗲𝗮𝘂𝘁𝗶𝗳𝘂𝗹𝗦𝗼𝘂𝗽 – For parsing HTML and extracting company names, email addresses, websites, phone numbers, and descriptions.

 • 𝗥𝗲𝗾𝘂𝗲𝘀𝘁𝘀 – For fetching static content when full browser rendering wasn’t needed, reducing load time.

 • 𝗽𝗮𝗻𝗱𝗮𝘀 – For organizing and exporting the extracted data in a clean tabular structure (CSV/Excel).

 • 𝗿𝗲 (Regular Expressions) – For validating and completing truncated or partially written email addresses (e.g., fixing emails like abc@domain...).



𝗢𝘂𝘁𝗰𝗼𝗺𝗲

 • Successfully extracted and cleaned contact information of over 𝟭,𝟱𝟬𝟬+ companies in the motorcycle spare parts industry.

 • The structured dataset significantly reduced manual outreach efforts and accelerated supplier discovery.

 • The scraping engine was designed to be 𝗸𝗲𝘆𝘄𝗼𝗿𝗱-𝗮𝗴𝗻𝗼𝘀𝘁𝗶𝗰, meaning it can be reused for different industries by just changing the search term.

 • Included handling of edge cases like paginated results, incomplete emails, and retry mechanisms for failed loads.
