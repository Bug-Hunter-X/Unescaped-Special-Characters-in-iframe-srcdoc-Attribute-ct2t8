# Unescaped Special Characters in iframe srcdoc Attribute

This repository demonstrates a bug related to unescaped special characters in the `srcdoc` attribute of an HTML `iframe` element.  The issue arises when attempting to embed HTML content containing characters like `<` or `&` without proper escaping.

## Bug Description

The `srcdoc` attribute allows embedding HTML content directly into an iframe. However, if the embedded HTML contains unescaped special characters, they may not render correctly, resulting in unexpected behavior or incorrect display of the content.  The iframe might display the raw HTML code instead of the intended formatted text.

## Solution

The solution is to properly escape the special characters within the `srcdoc` attribute using HTML entities.  For example, replace `<` with `&lt;` and `&` with `&amp;`.

## How to Reproduce the Bug

1. Open `bug.html` in a web browser.
2. Observe the incorrect rendering of the text within the iframe.

## How to Fix the Bug

1. Open `solution.html` in a web browser.
2. Observe the correctly rendered text within the iframe, demonstrating the corrected use of HTML entities for character escaping.