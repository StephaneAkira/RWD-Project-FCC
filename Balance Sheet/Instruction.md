- Screen readers announce HTML elements based on the document flow. We will eventually want the balance sheet to have a heading of "Balance Sheet" and a subheading of "AcmeWidgetCorp". However, this order does not make sense if announced by a screen reader.

- Give your existing span the class attribute set to flex, and add two span elements within it. Give the first the text AcmeWidgetCorp. Give the second the text Balance Sheet. You will use CSS to reverse the order of the text on the page, but the HTML order will make more sense for a screen reader.

- Below your h1 element, create a div element. Give it an id attribute set to years. You want this particular element to be hidden from screen readers, so give it the aria-hidden attribute set to true.

- Within your div element, add three span elements. Give each of them a class attribute set to year, and add the following text (in order): 2019, 2020, and 2021

- Below your existing div element, add a new div element with a class set to table-wrap. This will be the container for your tables.

Within that, add three table elements. You will be using CSS to style these into a single table, but using separate tables will help screen readers understand the document flow.

- HTML tables use the caption element to describe what the table is about. The caption element should always be the first child of a table, but can be positioned with the caption-side CSS property.

Add a caption element to your first table, and give it the text Assets

- The thead and tbody elements are used to indicate which portion of your table is the header, and which portion contains the primary data or content.

Add a thead and tbody to your first table, below the caption element.

- The tr element is used to indicate a table row. Add a tr element within your thead element. In your new tr element, add a td element, followed by three th elements.

The td element indicates a data cell, while the th element indicates a header cell.

- Within each of your new th elements, nest a span element with the class set to sr-only year. Give them the following text (in order): 2019, 2020, and 2021.

Give your third th element the class attribute set to current.

Leave the td element empty. This element exists only to ensure your table has a four-column layout and associate the headers with the correct columns.

- Within your tbody element, add four tr elements. Give the first three a class attribute set to data, and the fourth a class attribute set to total.

- In your first tr, add a th element with the text Cash This is the cash we currently have on hand.. Wrap all of that text except Cash in a span element with the class set to description.

Following that, add three td elements with the following text (in order): $25, $30, $28. Give the third td element a class attribute set to current.

- In your second tr element, add a th element with the text Checking Our primary transactional account.. Wrap that text, except for Checking , in a span element with the class attribute set to description.

Following that, add three td elements with the following text (in order): $54, $56, $53. Give the third td element a class attribute set to current.

- In your third tr element, add a th element with the text Savings Funds set aside for emergencies.. Wrap that text, except for Savings , in a span element with the class attribute set to description.

Following that, add three td elements with the following text (in order): $500, $650, $728. Give the third td element a class attribute set to current.

- In your fourth tr element, add a th element with the text Total Assets. Wrap the text Assets in a span element with the class attribute set to sr-only.

Following that, add three td elements with the following text (in order): $579, $736, $809. Give the third td element a class attribute set to current.
