# APC-PPID

Nowadays, the most commonly used type of code injection is Reflective ones. This is due to high levels of stealth and Meterpreter, Beacon etc. projects support this type of injection. There is a rule: if something is popular, the defenders focus on it. I've seen so little that this rule has changed. Many studies have been done to capture the techniques of Reflective injections. I also do not prefer to use the popular things in red team operations at the first stage to avoid attracting attention.

This code adds a user-mode asynchronous procedure call (APC) object to the APC queue of the thread of the created process and spoof the Parent Process. So, you can do APC Injection with the code I shared and spoof the Parent Process as explorer.exe. The execution flow of the project is given below.

![](https://raw.githubusercontent.com/hlldz/APC-PPID/master/execFlow.png)

## Acknowledgements and References
* https://blog.xpnsec.com/becoming-system/
* https://www.countercept.com/blog/detecting-parent-pid-spoofing/
