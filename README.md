# Begginer-Workmanager

WorkManager is an API that makes it easy to schedule deferrable, asynchronous tasks that are expected to run even if the app exits or the device restarts. 

Work Manager is a componet of android JETPACK and it is bassically for scheduking background task. Task may run immediately or an appropriate time.
Example:-  Backing up data to the server etc

**The Classes**

**worker** --  The work needed to be done is define here

**workRequest**--  it define the work , like which worker class is going to be execute, the **workRequest** class is a abstruct class, so we will use direct subclasses. **OneTimeWorkrequest** or **PeriodicWorkRequest**

**workManager**--  it enqueue and manage the work request

**workInfo**-- It contain the information of work like **workId,work status**


In this example we create **OneTimeWorkrequest** work with sending and receiving data and **Constraints** 


**PeriodicWorkRequest**  -- MIN_PERIODIC_INTERVAL_MILLIS 900000 **(15 mints)**
