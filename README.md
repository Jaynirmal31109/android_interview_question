# Android Interview Question 2023
### 1. What are the memory leaks? What are the best practice to avoid memory leak in android? ###
👉  A memory leak happen when memory allocated but never trash.\
    There are so many things to take note for avoid memory leaks.\
    * Broadcast Receivers: We need to register broadcast receiver, but if we don't unregister same then it holds the refrence even when activity/fragment         distroy.\
    
