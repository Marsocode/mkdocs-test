# Dictionary
_________________

## Cold App Start
A cold start refers to an app's starting from scratch: the system’s process has not, until this start created the app’s process. It happens when your app is being launched for the first time since the device booted, or since the system killed the app.

#### Sample use case
* Hold your mobile device
* Close all your opened apps
* Click on your app icon from home
* Everything will be initialized from zero
‍

According to [Google](https://developer.android.com/topic/performance/vitals/launch-time), the ideal benchmark time should be: 

* [Cold](https://developer.android.com/topic/performance/vitals/launch-time#cold) startup takes 5 seconds or longer.
* [Warm](https://developer.android.com/topic/performance/vitals/launch-time#warm) startup takes 2 seconds or longer.
* [Hot](https://developer.android.com/topic/performance/vitals/launch-time#hot) startup takes 1.5 seconds or longer.
_________________

## Connection
Line connecting two slices showing what previous function triggered the execution of the selected function.
_________________

## Hot App Start
A hot start refers to when your apps’ process is already running in the background and all the system does is bring your activity to the foreground. This process will bring back your app to the last state where you left without reinitializing any of the app assets.

### Sample use case
* Hold your mobile device
* Close all your opened apps
* Click on your app icon from home
* Everything will be initialized from zero
* This was so far for a cold start
* Go back to home
* Re-open the app again
* Your app is now bring back to the foreground without reinitialization

According to [Google](https://developer.android.com/topic/performance/vitals/launch-time), the ideal benchmark time should be: 

* [Cold](https://developer.android.com/topic/performance/vitals/launch-time#cold) startup takes 5 seconds or longer.
* [Warm](https://developer.android.com/topic/performance/vitals/launch-time#warm) startup takes 2 seconds or longer.
* [Hot](https://developer.android.com/topic/performance/vitals/launch-time#hot) startup takes 1.5 seconds or longer.
_________________

## Instrumentation
Instrumentation is the method in which our plugin can extract the necessary information about the runtime of the application, such as, how long functions run, which processes they call (child or async) and which threads they run on. It runs during the build process, instrumenting by injecting 100% of all functions and frameworks automatically without sampling.
_________________

## Slices
The visual representation of a code’s function/process. The length of the slice indicates how long it takes that process to execute.

The width of the slice represents the duration of the executed process and its position indicates the start time.

‍![slice name](./images/dictionary/slices.png)
_________________

## Trace
Think of a trace as the technical representation of a mirror showing us the user's journey. It includes hardware and software advances occurring through an entire app stack. 

The trace viewer will show vital information such as what functions were invoked, their duration, and most importantly, their execution paths. The visualization of execution paths is crucial because it allows everyone to see the sequence of functions and how they connect and highlight optimization opportunities.
_________________

## (User) Flow
Flow is the path a user takes to complete a task within the app. For example, the user types in “restaurant near me”. The app then returns search results. Finally, the user viewing searched results is considered a flow.

‍![user flow diagram](./images/dictionary/user_flow_1_modal.png)