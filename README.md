# YouTube URL Parser

This Python project, implemented in the `watch.py` file, facilitates the extraction of YouTube video URLs from HTML code containing iframe elements. The `parse` function takes a string of HTML as input, identifies any YouTube URLs within the src attribute of an iframe element, and returns their corresponding shorter, shareable youtu.be equivalents. If no such URL is found, the function returns None.

## Usage
1. Run the program by executing `python watch.py`.
2. Input the HTML code containing an iframe element with a YouTube URL as its src attribute.
3. The program will output the shorter, shareable youtu.be URL equivalent.

## Functionality
- **HTML Parsing:** The `parse` function utilizes regular expressions to extract YouTube URLs from the src attribute of an iframe element in the provided HTML string.
- **URL Transformation:** It transforms the extracted YouTube URL to its shorter, shareable youtu.be equivalent.
- **Error Handling:** The program handles cases where the input HTML does not contain a YouTube URL and appropriately returns None.

## How to Test
Manually test your code using the following steps:
1. Run your program with `python watch.py`.
2. Input HTML containing an iframe element with a YouTube URL in one of the specified formats.
3. Verify that the program correctly extracts and outputs the shorter, shareable youtu.be URL.

Example:
```html
<iframe src="http://www.youtube.com/embed/xvFZjo5PgG0"></iframe>
```
Expected Output:
```
https://youtu.be/xvFZjo5PgG0
```

```html
<iframe width="560" height="315" src="https://www.youtube.com/embed/xvFZjo5PgG0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
```
Expected Output:
```
https://youtu.be/xvFZjo5PgG0
```

```html
<iframe width="560" height="315" src="https://cs50.harvard.edu/python"></iframe>
```
Expected Output:
```
None
```

Ensure to test the program using the provided check50 command for additional verification.

## Creator
- **Name:** [Bassam Mejlaoui]
- **LinkedIn:** [https://www.linkedin.com/in/bassam-mejlaoui/]
- **GitHub:** [https://github.com/mejbass]
- **Portfolio:** [https://www.datascienceportfol.io/BassamMejlaoui]
