# Text Alignment Function

This JavaScript function `solution(paragraphs, aligns, width)` aligns text paragraphs within a specified width and adds a border. Here's a breakdown of the function:

## Function Parameters

- `paragraphs`: An array of arrays, where each inner array contains words for a paragraph.
- `aligns`: An array of alignment instructions ('LEFT' or 'RIGHT') for each paragraph.
- `width`: The maximum width of each line.

## How It Works

1. The function starts by creating a border using asterisks.
2. It then processes each paragraph:
   - Words are combined into lines, respecting the maximum width.
   - Each line is aligned according to the specified alignment (left or right).
3. The aligned text is enclosed within asterisks.
4. Finally, it adds a closing border.

## Usage Example

```javascript
const paragraphs = [["hello", "world"], ["how", "are", "you", "doing"]];
const aligns = ["LEFT", "RIGHT"];
const width = 16;

const result = solution(paragraphs, aligns, width);
console.log(result.join('\n'));
```

## Output

```
******************
*hello world     *
*          how   *
*         are    *
*         you    *
*        doing   *
******************
```

## Notes

- The function handles both left and right alignment.
- It automatically wraps text to fit within the specified width.
- The border width adjusts based on the specified `width` parameter.

This function is useful for formatting text in scenarios where you need to create aligned, bordered text blocks, such as in console applications or text-based user interfaces.
