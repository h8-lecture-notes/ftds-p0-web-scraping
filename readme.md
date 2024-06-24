# Web Scraping

- Web Scraping is a data retrieval/extracting technique by leveraging the use of HTML language in a website.
- HTML is a standard language to create the structure of a website.
- HTML consists of `Element(s)` that define the structure, layout, and formatting of the content on a website.
- An `Element` is defined by a `<tag_name> some content </tag_name>`
- Example of HMTL `Element(s)`:
  - `<html>...</html>`
  - `<body>...</body>`
  - `<title>...</title>`

    > `<title>` -> start tag
    >
    > `...` -> element content
    >
    > `</title>` -> end tag
  - read more <https://www.w3schools.com/html/html_elements.asp>

## How to scrape data

- Before scarping data from HTML, we usually look for the target tag and its attribute (if necessary) of the element that we want to extract.
  - Example:

    ```html
    <html>
        <body>
            <h1>Lorem Ipsum</h1>
            <ul class='list-data'>
                <li id='data1'>dolor</li>
                <li id='data2'>sit</li>
                <li id='data3'>amet</li>
            </ul>
        </body>
    </html>
    ```

    > if we want to extract "Lorem Ipsum" text, then we need to target an element with `<h1>` tag.
- Scraping in python can be perform using these packages:
  - Selenium <https://pypi.org/project/selenium/>
  - BeautifulSoup <https://pypi.org/project/beautifulsoup4/>

## Requirements

- Make sure Selenium and BeautifulSoup4 installed:

    ```bash
    # install packages using pip
    pip install selenium beautifulsoup4
    
    # optional
    pip install requests
    ```
