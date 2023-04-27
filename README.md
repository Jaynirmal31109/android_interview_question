# Android Interview Question 2023
### 1. What are the memory leaks? What are the best practice to avoid memory leak in android? ###
👉  A memory leak happen when memory allocated but never trash.\
There are so many things to take note for avoid memory leaks.
  * Broadcast Receivers: We need to register broadcast receiver, but if we don't unregister same then it holds the refrence even when activity/fragment     distroy.
* Avoid usages of static variables.
* We need to use getApplicationContext() where we need to get the context in application insted of activity context. If we need to use activity context then we need to destroy them on activity destroy.
* Distroy asynctask and other bacground theread task while activty distroy. It will initiate to memory leak.
    
