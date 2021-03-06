# Troubleshooting

This page contains some advice about errors and problems commonly encountered during the development of jCrystal applications.

## Nothing happens when I run jCrystal

Remember that jCrystal will only generate code if it finds anything that can generate for you. Therefore, in an empty project, nothing will happen if you run jCrystal. 
To check that jCrystal is running:

1. Open the console view by going to `Window > Show View > Console`. Clear the console. 

2. Go to your Package Explorer, select your project and: 
- Pressing  `CTRL + 6` (Windows) or `CMD + 6` (Mac OS).

    or
- Pressing the jCrystal icon. <img src="../images/logo_min.png" alt="jCrystal Logo">

3. On your console you should see something like:

```
UTF-8
Time sending (11): 147 ms
Total time: 804 ms
```

Even if nothing is happening, if you see these lines jCrystal is running as expected. If you have an empty project and want to see jCrystal in action [learn how create your first webservice and run your application](run_test.md). 

If on the console logs you see any line that starts with "Server error message", please check: 
- [Server error message: Invalid key or not given](#server-error-message-invalid-key-or-not-given)
- [Server error message: XXX](#server-error-message-xxx)


## jCrystal doesn't generate anything and it should
If you have checked [nothing happens when I run jCrystal](#nothing-happens-when-i-run-jcrystal) and jCrystal is running as expected but it's not generating anything. Then,

- Make sure you have saved all your files.
- Refresh your project by going to `File > Refresh`.
- Update your depedencies by right-clicking your new project and selecting `jCrystal > Add dependencies`. 
- Try running jCrystal once again. 

## jCrystal throws SocketTimeoutException: Read timed out
This exception occurs whenever there's a timeout with jCrystal server. Please check your internet connection and try running jCrystal once again.

## Server error message: Invalid key or not given
This error occurs when the key of the project hasn't been properly set. Please check [how to create and setup the key.](creating_project.md#create-and-setup-a-key)

## Server error message: XXX

- Update your plugin by going to `Help > Check for updates`.
- Update your depedencies by right-clicking your new project and selecting `jCrystal > Add dependencies`. 
If none of this solutions work, please contact us.
