Link: https://ctflearn.com/challenge/220


![image](https://user-images.githubusercontent.com/94149390/174475412-33f2c08e-60a2-411d-b828-a1741199f5f7.png)

**Step 1:** 

I download file from: https://mega.nz/#!jexRzTzD!Fd3tD8ZcLquXJrsycMFUzozC9MHqaG-srUBfGREtL-0

**Step 2:**

I open [hereisyourflag.m4a](https://github.com/kietbl/Research/blob/main/Music%20To%20My%20Ears/hereisyourflag.m4a) but it is corrupted.

So, I use Faad and Faac to fix it.

You can download Faad [here](https://rarewares.org/aac-decoders.php) and Faac [here](https://rarewares.org/aac-encoders.php)

**Step 3:**

Make sure Faac, Faad and [hereisyourflag.m4a](https://github.com/kietbl/Research/blob/main/Music%20To%20My%20Ears/hereisyourflag.m4a) are in the same place.

I open [it](https://github.com/kietbl/Research/blob/main/Music%20To%20My%20Ears/hereisyourflag.m4a) with Hex Editor.

Next, I press Ctrl F and type "mdat" into search bar.

![image](https://user-images.githubusercontent.com/94149390/174476280-6f0a5e0e-2dab-42fa-9ce7-8a8449f85f9d.png)

Select from beginning to "mdat" tag.

![image](https://user-images.githubusercontent.com/94149390/174476556-308c4631-e516-41ee-a39c-1106a6380d82.png)

and delete all of it.

Ctrl S to save file.

**Step 4:**

Using Faad to decode file.

Using cmd, cd to the folder that contain Faad, Faac and [hereisyourflag.m4a](https://github.com/kietbl/Research/blob/main/Music%20To%20My%20Ears/hereisyourflag.m4a)

Type ***faad.exe "hereisyourflag.m4a"***

![image](https://user-images.githubusercontent.com/94149390/174476741-fa505095-7f65-4869-a282-71e0ae5caf79.png)

the file will decode to ***hereisyourflag.wav***

**Step 5:**

In cmd, type ***faac.exe -b 160 -o repaired.m4a “hereisyourflag.wav”*** (you can replace "repaired.m4a" with any name you like)

You will get file name "repaired.m4a".

**Step 6:**

Open repaired.m4a and listen to the flag ;)

Flag: 
>CTFLearn{1_c4n_f1x_it}

Note: You can open ***hereisyourflag.wav*** to listen to flag, but if you want to know how to encode and fix m4a file, you should follow **Step 5**. 

