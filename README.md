<h1>Readers' Corner — Web Scraping Datasets</h1>
<p>CS4048 Data Science — Assignment 1, Version B. Two datasets scraped in Python.</p>

<h2>1. Bookstore Catalog</h2>
<p><strong>Site:</strong> <a href="https://books.toscrape.com/index.html">books.toscrape.com</a><br>
<strong>Tools:</strong> <code>requests</code> + <code>BeautifulSoup</code><br>
<strong>File:</strong> <code>23L_2596_versionB_static_books.csv</code></p>

<p>Scraped 4 categories — Travel, Mystery, Historical Fiction, Classics — including every book's product page.</p>

<p><strong>Columns:</strong> Title, Price, Availability, Star rating (1–5), UPC, Description, Category</p>

<table>
<tr><th>Category</th><th>Books found</th><th>Result</th></tr>
<tr><td>Travel</td><td>11</td><td>PASS</td></tr>
<tr><td>Mystery</td><td>32</td><td>PASS</td></tr>
<tr><td>Historical Fiction</td><td>26</td><td>PASS</td></tr>
<tr><td>Classics</td><td>19</td><td>PASS</td></tr>
</table>
<p>88 books total before removing duplicates across categories.</p>

<h2>2. Inspirational Quotes (infinite scroll)</h2>
<p><strong>Site:</strong> <a href="https://quotes.toscrape.com/scroll">quotes.toscrape.com/scroll</a><br>
<strong>Tools:</strong> <code>Selenium</code><br>
<strong>File:</strong> <code>23L_2596_versionB_dynamic_quotes.csv</code></p>

<p>Raw HTML has 0 quotes — content loads via JavaScript. Used Selenium to scroll and collect quotes with explicit waits, stopping after 2 scrolls in a row with no new content.</p>

<p><strong>Columns:</strong> Quote text, Author, Tags, Number of tags, Scroll batch first seen</p>

<h2>Notes</h2>
<ul>
<li>Datasets are generated only by running the scrapers — no manual edits.</li>
<li>Full methodology is in <code>23L_2596.ipynb</code>.</li>
</ul>

</body>
</html>
