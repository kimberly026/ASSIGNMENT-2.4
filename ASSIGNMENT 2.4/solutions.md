

# Assignment 2.4 — HTML Validation & Debugging



```

<!DOCTYPE html>
<html>
<head>
    <title>My College Webpage<title>
</head>
<body>
    <h1>Welcome to My College
    <p>Our college provides quality education.
    <div>
        <h2>Our Departments</h2>
        <ul>
            <li>Computer Science
            <li>Mechanical Engineering</li>
            <li>Electrical Engineering</li>
        </ul>
    <p>Visit our college website:
    <a href="https://example.com">Click here</p>
    <img src="college.jpg">
</body>
</html>

```

### Illustration 1: Understanding the debugging task

Buggy HTML file

Missing tags, incorrect nesting, and missing attributes

Inspect and validate

Use browser DevTools and an HTML validator

Corrected HTML file

Proper nesting, closing tags, attributes, and indentation

## 3. Identification of errors

After examining the code, the following errors can be identified.

| No. | Error                                                                                    | Correction                                     |
| --- | ---------------------------------------------------------------------------------------- | ---------------------------------------------- |
| 1   | The `<title>` tag is not closed correctly.                                               | Use `</title>`.                                |
| 2   | The `<h1>` heading has no closing tag.                                                   | Add `</h1>`.                                   |
| 3   | The first paragraph has no closing tag.                                                  | Add `</p>`.                                    |
| 4   | The `<div>` container is not closed.                                                     | Add `</div>` before the next section.          |
| 5   | The first list item has no closing tag.                                                  | Add `</li>`.                                   |
| 6   | The second paragraph is not closed.                                                      | Add `</p>`.                                    |
| 7   | The anchor tag is incorrectly nested inside a paragraph without a proper closing `</a>`. | Close the anchor before closing the paragraph. |
| 8   | The image has no `alt` attribute.                                                        | Add descriptive alternative text.              |
| 9   | The code indentation is inconsistent.                                                    | Indent nested elements consistently.           |

Note: Some HTML errors can be automatically repaired by the browser when it builds the page. However, the original source code still needs to be corrected. The `alt` attribute is important for accessibility, while consistent indentation makes the code easier to read and maintain.











## 6. Corrected HTML file (After debugging)

The following is the corrected version of the webpage. Save it as `index.html`.

```

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My College Webpage</title>
</head>
<body>
    <header>
        <h1>Welcome to My College</h1>
        <p>Our college provides quality education.</p>
    </header>

    <main>
        <section>
            <h2>Our Departments</h2>
            <ul>
                <li>Computer Science</li>
                <li>Mechanical Engineering</li>
                <li>Electrical Engineering</li>
            </ul>
        </section>

        <section>
            <h2>More Information</h2>
            <p>
                Visit our college website:
                <a href="https://example.com">Click here</a>
            </p>
            <img
                src="college.jpg"
                alt="College building"
                width="400"
            >
        </section>
    </main>
</body>
</html>

```

### Explanation of the corrections

- `</title>` properly closes the page title.
- `</h1>` closes the main heading.
- `</p>` closes each paragraph.
- `</div>` is no longer needed because the corrected layout uses semantic `<header>`, `<main>`, and `<section>` elements with proper closing tags.
- Every list item has an appropriate closing tag.
- The anchor uses a correctly closed `<a>` element.
- The image includes `alt="College building"` and a width attribute.
- The `lang="en"` attribute specifies the document language.
- The character encoding and viewport meta tags improve compatibility and mobile display.
- The indentation makes the hierarchy of elements easier to understand.



