# ***PICO CTF 2019***

1. GLory of the Garden
   * The text is present in the image.
   * Get the flag by typing the following in terminal
    ```bash 
    strings garden.jpg | grep picoCTF
    ```

2. The Numbers
    * View the image by typing 
    ```bash
    xdg-open the_numbers.png
    ```
    * The flag will show in the image
    * Convert the numbers to letters
    * They are similar to the sequence of alphabet values
    * eg. A=1, B=2, .... etc
    * You'll get the flag after conversion

3. practice-run-1
    * Make the file executable by typing
    ```bash
    chmod u+x run_this
    ```

    * Followed by the next line to execute it
     ```bash
    ./run_this
    ```

4. unzip
    * unzip the file by typing
    ```bash
    unzip flag.zip
    ```
    * You'll get an extracted image
    * Type 
    ```bash 
    xdg-open flag.png
    ```
    * The flag will show in the image

5. vault-door-training
    * Open the java source code by typing
    ```bash 
    nano VaultDoorTraining.java
    ```
    * The flag will show in the source code in the last line of   * checkPassword function

6. 13-Points
    * The flag is rot13 encrypted 
    * Decrypt it by typing the following in terminal
    ```bash 
    echo 'cvpbPGS{abg_gbb_onq_bs_n_ceboyrz}' | tr 'A-Za-z' 'N-ZA-Mn-za-m'
    ```

7. Bases
    * The flag is encoded using base64
    * Decode by typing 
    ```bash 
    echo 'bDNhcm5fdGgzX3IwcDM1' | base64 -d
    ```
    * The flag will show

8. First Grep
    * Extract the flag from the file by typing
    ```bash 
    cat file | grep CTF
    ```

9. strings it
    * If we run cat command we get all garbage data
    * So we type the following to extract only strings from the data and also look for the word CTF
    ```bash 
    strings strings | grep CTF
    ```
    * The flag will show up

10. vault-door-1
    * Open the source code by typing 
    ```bash 
    nano VaultDoor1.java
    ```
    * The positions of various characters if the flag will show in the function below
    * They can be typed directl by viewing the positions or by using a script

11. Insp3ct0r
    * Open the website link and view the page source
    * 1/3rd of the flag will show in the last lines of page source
    * The other 2 parts of the flag are in the css and js links of the page source

12. Easy1
    * The text is encrypted using vigenere cipher
    * For each character in the key, Check the top row of the table for the corresponding character
    * Once found, go down that column till you find the corresponding letter of the encrypted text
    * The corresponding letter in the first column is your character

13. Resources
    * Open the website and scroll down
    * The flag will be below the video

14. dont-use-client-side
    * Open the source code of the website
    * The flag will be split up in the verify function

15. logon
    * Login with any random username and password
    * Once logged in open inspect element and go to storage tab to view cookies
    * Change the cookies value of admin to True and reload page
    * The flag will show on the screen

16. what's a netcat?
    * Type the following in terminal to connect using netcat
    ```bash 
    nc 2019shell1.picoctf.com  47229
    ```
17. So Meta
    * The flag is hidden in the metadata of the image
    * To view the metadata type the following in terminal
    ```bash
    identify -verbose pico_img.png 
    ```

18. where are the robots
    * robots.txt is a file in which developers put data which they don't want web crawlers to find
    * To view the file add /robots.txt at the end of the website url such that it looks like this https://2019shell1.picoctf.com/problem/32229/robots.txt
    * It will show what is disallowed
    * Add that disallowed part at the end of the url such that it looks like this https://2019shell1.picoctf.com/problem/32229/0ecd0.html
    * The flag will show up

19. What Lies Within
    * The flag is embedded within the image
    * The retrieve the flag type the following in terminal
    ```bash
    zsteg buildings.png
    ```

20. extensions
    * If we view the text file using cat or nano, we can see that it has unreadable text
    * Use file command to check file type by typing the following
    ```bash
    file flag.txt
    ```
    * It shows it's a PNG file
    * Open the text file in a image viewer
    * The flag shows in the image

21. Based
    * Run the given netcat command to connect to the server
    * Use online converters to convert the given data to text
    * The 1st is in Binary, 2nd is in Octal and 3rd is Hex

22. shark on wire 1
    * Open the capture in wireshark by typing
    ```bash
    sudo wireshark capture.pcap
    ```
    * Type udp in top bar
    * Select a udp stream packet, right click and select follow udp stream.
    * Keep changing the stream till you find the flag