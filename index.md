---
layout: default
---

Text can be **bold**, _italic_, ~~strikethrough~~ or `keyword`.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

![chopper](7144d67e51b17a56890aa002a750f3c7-2028755823.jpg)

# Building a Port Scanner

08/03/2025

First, I added some import lines to setup the information it can receive.
#img

Then I used an if else statement to define the target.
#img

Added a banner next to make it look slightly nicer.
#img

Next I used a try statement for what specific port range will be scanned. I chose the range of 50 and 85 because ports that range from 50-85 are commonly used in home routers such as DNS and HTTP. I then defined the s variable and used settimedefault so that it wouldn't spend more than 1 second scanning each port. I used result to tell me which ports were open and to close ports that were not. 
#img

I had to add exceptions to make the scanner exit properly if and interuption occured. I used KeyboardInterrupt in case of a Ctrl+C, socket,gaierror for an incorrect hostname, and socket.error for inablility to connect to an IP Address.

Here are the results for the first port scan using my home router.

![scannertest1](https://github.com/user-attachments/assets/76d94916-387c-40e0-b4de-bf222c91750e)

As you can see, it only came up with DNS and HTTP. I ran another test after this to check if 443 was as well and it was it was open as well.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](wp4628424-7998573.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
