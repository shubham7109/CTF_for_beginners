Ans : flag{steganography_is_the_bane_of_my_existance}

Solution:
Click this [link] (https://tnek.gitbooks.io/csaw-2015-hsf-preliminary-writeups/content/500_-_whats_the_difference.html) for the solution of this file.

OR

If we look at bane.png, we can see that there is actually another png hidden inside it.<br>
To find this out we can type 
> strings bane.png
in terminal and there will be 2 "PNG" file signatures which means that there are 2 images in the file.<br>
The second png looks the same, so let's compare the bytes to see "Whats the Difference".<br>

    $ compare first.png second.png -compose src diff.png

If we open up diff.png, we are greeted with a QR code. Scan it to get the flag.<br>

flag{steganography_is_the_bane_of_my_existance}

    


