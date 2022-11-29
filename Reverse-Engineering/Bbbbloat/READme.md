# Pico_CTF
## @author : M3tr1c_r00t
### Bbbbloat!
Bbbbloat is an easy challenge which requires on to be able to decompile the given binary and analyze it to be able to get the flag.

### Running the binary
First off, we're gonna get our binary from the site using wget and the link...

After marking the file executable (chmod +x your_binary), we can see that it's asking for input; asking for our favourite number.
![Screenshot_2022-11-20_21_23_53](https://user-images.githubusercontent.com/99975622/204566602-d24b394e-4495-4cba-bbce-ddd9e41c4f08.png)
On entering any random number, its responds with a error message saying that the number that we entered isn't the lucky number.

Next up, we fire up ghidra, which is a decompiler and will help us be able to get the source code of the given binary in either Assembly code and C like code.
<br>You can launch the ghidra framework by typing ghidra on the terminal.
<br>In case you had not downloaded it, it will ask you whether you'd like to install it or not:)
![Screenshot_2022-11-20_21_21_58](https://user-images.githubusercontent.com/99975622/204599020-6224b082-e959-4d9a-abaf-130968b10131.png)
Next up,we can create a project;
![Screenshot_2022-11-20_21_22_30](https://user-images.githubusercontent.com/99975622/204599146-f927c463-d853-4324-8c31-081986ac4f51.png)
Import your binary file and then click on the green dragon to start up your project.
<br>You can also import your binary after the project is started;
![Screenshot_2022-11-20_21_22_42](https://user-images.githubusercontent.com/99975622/204599549-c22ff1b1-a575-49cd-9e12-c13c7b5fbec3.png)
Jus click on files, and go to import;
![Screenshot_2022-11-20_21_22_56](https://user-images.githubusercontent.com/99975622/204599671-5a219758-53a3-48ba-a3bf-910312d7ea75.png)
After confirming the import , a pop up will appear asking whether to continue with the decompilation process, you can accept all.
### Binary Analysation
<br>After the decompilation process is through, we can now see a couple of panes in the framework. 
![Screenshot_2022-11-20_21_24_42](https://user-images.githubusercontent.com/99975622/204599952-0590dc1a-4783-4488-919f-85c27dd37a16.png)
On the right, we have the decompiled code from Assembly language.
<br>Next we have the middle pane containing the binary translation to Assembly
<br> And on the left, we have the binary functions and classes among others.
![Screenshot_2022-11-20_21_24_53](https://user-images.githubusercontent.com/99975622/204600698-3d6d7fd6-46c5-4a60-bd98-070d2e5aa675.png)

On the main function, we can see how the program runs.
<br>We can there's a hexadecimal number which is being used in an if else function.
<br>We can see the value of the number by typing it directly to python.

![Screenshot_2022-11-20_21_25_05](https://user-images.githubusercontent.com/99975622/204601414-326b044e-5dc0-4207-921c-4c47b8c16d1b.png)

And boom! We got our lucky number.
<br> We can now head over back to our terminal and see what response we'll get from this binary with this number.
![Screenshot_2022-11-20_21_25_18](https://user-images.githubusercontent.com/99975622/204601725-98ab1817-f727-421e-8bfd-516661ec1fb5.png)
And Done!
<br> We got our flag!
#### End!

### Socials
@Instagram:https://instagram.com/M3tr1c_r00t
<br>@Twitter:https://twitter.com/M3tr1c_root
