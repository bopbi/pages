# (DRAFT) Ideas for make own push messaging client for android, without firebase
###### Date: 2025/01/03

### Things to consider for implementation
* Android version, this related on how the android behavior in relation with the background limitation, some SDK version are quite loose and some require to use certain API
* Network Protocol : MQTT, this raise the question on how to authenticate it

### Idea 1 - Without Worker
*  use the JobService API (target is SDK 21)
*  need to acquire the wakeLock since technically it should operated in background
*  Logic for
### Idea 2 - With Worker
* this might an odd one, although the API (like scheduling, constraint) is quite convenience, the worker have a 10 minutes limitation execution
* OS can delay the execution
* 
---
