# cop3503-lab-8---numeric-conversion-solved
**TO GET THIS SOLUTION VISIT:** [COP3503 Lab 8 – Numeric Conversion Solved](https://www.ankitcodinghub.com/product/cop3503-lab-8-numeric-conversion-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;68768&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COP3503 Lab 8 – Numeric Conversion Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<h1>Overview</h1>
In this assignment you are going to read common color names and their corresponding numeric values from a group of files. One small issue: the numbers are in the wrong format. They are stored in integers, while typically color values are represented in one of two ways–either in hexadecimal form, or as their 3 separate color channels. For example, the color red might be represented like this:

0xFF0000 as hexadecimal

Red: 255, Green: 0, Blue: 0 as unsigned characters, or

Red: 1.0f, Green: 0.0f, Blue: 0.0f as floats

The integer representation of that color would be 16711680—this number is, at face value, useless. However, breaking that integer into multiple, individual pieces is often done. In this assignment, you are going to convert this not-so-helpful integer into a helpful hex value and RGB value. For more general information on color codes:

<a href="https://htmlcolorcodes.com/">https://htmlcolorcodes.com/</a> <a href="https://www.w3schools.com/colors/colors_names.asp">https://www.w3schools.com/colors/colors_names.asp</a>

<h1>Description</h1>
The six files to load are called <strong>colors1.txt</strong>, <strong>colors2.txt</strong>, etc up to <strong>colors6.txt</strong>. Each file contains a list of colors with their name and integer representation of the color. You are to write a small program that loads one or more of these files, converts the values to hex/RGB values, and stores the list of colors in a <strong>std::map</strong> object<strong>.</strong>

Storing multiple values in a single variable is a common thing in code. You may do this conserve memory, or to easily pass multiple values around without creating new classes to store them. Very commonly this will be for small values, such as characters or shorts, and they are stored in larger integer variables.

The way to store/retrieve these values is by <strong>bit-shifting</strong>.

Imagine a single byte (i.e. a signed or unsigned character), made up of 8 bits:

The number 12 in binary form: 0 0 0 0 1 1 0 0

The number 255 in binary: 1 1 1 1 1 1 1 1

If you wanted to store these two separate values in one 2-byte short (12 first, then 255), the bytes for that short would look like: 0 0 0 0 1 1 0 0 1 1 1 1 1 1 1 1. Its decimal value would be 3,327 which, has no obvious connection to either of the two values we’re storing. All of memory is like this, but fortunately for programmers we can deal with memory one variable at a time.

If we took a short, and initialized it to 12, its bytes would be 0 0 0 0 0 0 0 0 0 0 0 0 1 1 0 0. Look at all that empty space on the left! So much room, you can store all kinds of things in there! (All kinds of things, as long as those things are bits.) If you want to store the 12 “on the left” you would left-shift the value. Each time you shift a value, its bits move over as many bits as you specify.

One thing you might notice is that bit-shifting multiplies or divides the value—left-shifting multiplies, while right-shifting divides. The amount of the modification is 2 to power of the number of bits by which you shifted. So left-shifting by 3 multiplies by 2<sup>3</sup>, while right-shifting by 2 would divide by 2<sup>2</sup>.

If you wanted to store the value of 12 in the “high byte” you would need to move the value over one byte, or 8 bits.

&nbsp;

For this assignment, you will be employing this concept to retrieve 3 unsigned char values from a single integer value. The integer is a 32-bit variable, and you will be retrieving values from bits 0-7 (the blue value), bits 8-15 (the green value), and bits 16-23 (the red value). Visually this would look like the following:

&nbsp;

In addition to storing values, you will need to retrieve those byte-values from the variable. This can be done by shifting and comparing to some known value, using the bitwise &amp; operator. The &amp; operator will compare two values, and every bit that is turned on (set to 1) in BOTH values will be present in the final result. For example:

&nbsp;

Retrieving the green value would be a similar process, by shifting the original value 8 bits, and the blue value wouldn’t need to be shifted at all before the &amp; comparison. After you’ve shifted and ANDed, you store the value in an unsigned char, and that’s it! If you wanted to put the value back in, you could start at zero, and then add the red value left-shifted by 16 bits, the green value left-shifted 8 bits, and then the blue value. If you were using an alpha value, that would be shifted by 24 bits.

<h1>Hexadecimal Conversion</h1>
After converting your colors to RGB, you will have to store it in a string representing the hexadecimal equivalent. Color values are often represented as hexadecimal numbers, with 2 letters each for the red, green, and blue values. Color values in character form range from 0-255, which can be stored in two hexadecimal digits, 0-FF. The color green would be 0x00FF00, blue would be 0x0000FF, a dark purple color with a value of 93, 0, 106 would be #5D006A.

Hexadecimal is base 16, which means each digit has a value from 0-15, or 0-9, then A is 10, B is 11, C, D, E, and F is 15. The first digit contributes its value to the total value of the number, the second digit contributes 16<sup>1</sup> times the value of the digit to the total of the number, and so on. For example, a value of F3 is (15∗16<sup>1</sup>)+(3∗16<sup>0</sup>), or 243.

<h2>Example</h2>
Because we’re dealing with numbers with a maximum value of 255 (and thus just 2 hex digits), the process for this is pretty straightforward:

Take your number and divide it by 16. The result is the number you want to convert to the first digit in the hex number. If the value is 0-9, then use that number as-is. If the number is 10-15, you need to convert it to the letters A-F.

<table width="623">
<tbody>
<tr>
<td width="62">Decimal</td>
<td width="37">0</td>
<td width="37">1</td>
<td width="37">2</td>
<td width="37">3</td>
<td width="37">4</td>
<td width="37">5</td>
<td width="37">6</td>
<td width="37">7</td>
<td width="37">8</td>
<td width="36">9</td>
<td width="32">10</td>
<td width="32">11</td>
<td width="32">12</td>
<td width="32">13</td>
<td width="32">14</td>
<td width="32">15</td>
</tr>
<tr>
<td width="62">Hex</td>
<td width="37">0</td>
<td width="37">1</td>
<td width="37">2</td>
<td width="37">3</td>
<td width="37">4</td>
<td width="37">5</td>
<td width="37">6</td>
<td width="37">7</td>
<td width="37">8</td>
<td width="36">9</td>
<td width="32">A</td>
<td width="32">B</td>
<td width="32">C</td>
<td width="32">D</td>
<td width="32">E</td>
<td width="32">F</td>
</tr>
</tbody>
</table>
&nbsp;

After that, you want to get the <strong>remainder</strong> of the original division to use as the second digit. For that, you can use the <strong>modulus operator</strong>. Take the result of the modulus operation and convert that number to a hex digit as well.

Take the number 243 (which should be F3 in hex):

243 / 16 = 15, with a remainder of 3 (16 * 15 = 240)

15 in hex is F

243 % 16 = 3, the remainder

3 in hex is just 3

If you were storing that in a std::string variable, string[0] would be the character ‘F’, and string[1] would be ‘3’. You could use the .resize() function to allocate space for 2 characters in the string, or you could assign it a default string of “00” and overwrite the two characters afterward—the std::string class has the subscript operator overloaded to access/modify individual elements of the string.

<h1>Color Class</h1>
The Color class you will write for this assignment is pretty simple. You will need to store the <strong>name</strong> and <strong>hex value</strong> of the color as <strong>std::strings</strong>, and the <strong>RGB values</strong> as <strong>unsigned characters</strong>. You should have the following functions in your class. Any other supporting functions/variables you want to create are up to you.

&nbsp;

<strong>/* Insert any other functions/data members that you want */ </strong>

<h1>Searching</h1>
After you have loaded and stored the colors, there will be an option to print everything or search for a single color by its name (the key in the std::map object). If the entered string is found in the map (using the find() function, refer to previous slides/lectures on searching for key/values in a std::map), print out the Color. If not, simply print out that their entry was not found. For example, if the user searched for the color “MintGreen” and it wasn’t found, print out:

MintGreen not found!

<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><strong>&nbsp;</strong>

<h1>Example Output</h1>
The output for files 1 and 2 are given so you can test your code against different sets of data. Each other file follows exactly the same format, though of the number of colors in each are different.

<img data-recalc-dims="1" decoding="async" data-src="https://i0.wp.com/www.ankitcodinghub.com/wp-content/uploads/2021/07/521.png?w=980&amp;ssl=1" src="data:image/gif;base64,R0lGODlhAQABAAAAACH5BAEKAAEALAAAAAABAAEAAAICTAEAOw==" class="lazyload">
