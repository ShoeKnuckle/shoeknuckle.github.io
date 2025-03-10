---
layout: default
---
[comment]: <> (Text can be **bold**, _italic_, ~~strikethrough~~ or `keyword`
There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.)
[comment]: <> ([Link to another page](./another-page.html))

# Building a Port Scanner

08/03/2025

First, I added some import statements to allow information to be received such as datetime. Then I used an if else statement to define the target and limit the user to two argument being "scanner.py" and the "IP". I also just added a banner next to make it look slightly nicer and to diplay the current date and time.

![image](https://github.com/user-attachments/assets/f3efc634-42d7-48af-97d0-d61e3f600b7e)

Next I used the try command and a for loop what specific port range will be scanned. I chose the range of 50 and 85 because ports that range from 50-85 are commonly used in home routers such as DNS and HTTP. I then defined the s variable and used settimedefault so that it wouldn't spend more than 1 second scanning each port. I used result to tell me which ports were open and to close ports that were not. I had to add exceptions to make the scanner exit properly and if an interuption occured. I used KeyboardInterrupt in case of a Ctrl+C, socket,gaierror for an incorrect hostname, and socket.error for inablility to connect to an IP Address. Below is the final script and the results for the first port scan, using my default gateway address to scan my home router.

![image](https://github.com/user-attachments/assets/f2058142-202f-4224-bb2c-f71cc2bae3ef)  ![scannertest1](https://github.com/user-attachments/assets/76d94916-387c-40e0-b4de-bf222c91750e)

As you can see, it only came up with DNS and HTTP. I ran another test after this to check if 443 was as well and it was it was open as well.


# Very Basic Calc

To start off, I put two imput statements in to give the user two numbers to calculate. I then added an input inbeteen so the user could choose an operator to use for their numbers:

![image](https://github.com/user-attachments/assets/88e8814d-6a59-4dbb-93f2-fb9c0aca4db8)

I then had to add the operators for the user so I just added +, -, /, *, and ** using an if else statement for the script to actually run. I added the option of using "^" to the "**" operator because people tend to use both. Final result:

![image](https://github.com/user-attachments/assets/13e54c3e-1e27-4319-a4f4-ac79d05fd444)


# Shoe Budget App 

I started this project by creating a class and defining the name and price of said "shoe" with an init statement, adding float to price incase of decimals. Then I defined a budget check using 'if not isinstance' so if the user typed sn invalid value, it will close down the application. I also had to define 'change' as budget - the self.price for an accurate amount of change to be received:
![image](https://github.com/user-attachments/assets/d69f834a-331b-4b83-8194-a4bac631541a)

Next, as shown above, I defined the buy option using an if else statement, so that as long as the budget is greater than the price of the shoe, the shoe can be purchased. If the budget is equal to the price, it can be purchased, and if the budget is higher, the change will be calculated. If the budget is lower than the price, the application will shut down:

![image](https://github.com/user-attachments/assets/1919c26d-83b7-41ca-98e6-84e4b05658c2)

In attempt to follow the DRY approach, I started another script. I firstly started using from Shoes import Shoes so I could use the data from the other script. The try statement was added nextfor the user to input the amound and if invalid, will be asked for a valid number. When I added the 'for' statement, I had to make sure the order or price was high, medium, low in that specific order. If I had it in the opposite oreder, no matter how much money the user has, it would always just choose the low option because it's the first option in order:

![image](https://github.com/user-attachments/assets/046211db-cb65-46bf-b948-ec88a096a697)

A few examples of possible outputs:
![image](https://github.com/user-attachments/assets/d09f8472-4301-4d1d-a801-3411db5599c9)
![image](https://github.com/user-attachments/assets/2d0bd90f-cb76-4b36-97de-66fe8a2bff25)
![image](https://github.com/user-attachments/assets/d752a5ae-b500-40b4-a731-18900ed97a48)



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
