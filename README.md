# SurvA

SurvA (pronounce "Survey") is An Open Source JAVA WatchDog proposal, aimed to provide a fast and lightweight solution in order to: 
- create any recursive pluggable survey task (of any kind). For instance: Connect to any network system in order to validate its availability (via HTTP, SOAP, any internal memory verification API
- manage alerts/notifications plans Initially based on a simple standalone JAVA SE threading and proprietary notification system, the system configuration was XML based in order to avoid any external dependency.

The new SurvA factoring tends to: 
- try and use dedicated Job Schedulers (e.g: Quartz Job Scheduler: http://www.quartz-scheduler.org/ ) 
- generate notifications through an asynchronous third party provider. 

This notifying aspect will be left up to Camel endpoints definition, so that any external notification module may be pluggable using MessageQueues.


Obviously, the aim is quiet close to the nagios-core Community project and  the dilema reamains between directly discovering and using Nagios (https://www.nagios.org/projects/nagios-core/) or building a self-made micro framework.

Therefore, as a disclosure: may this repository may also become part of personnal proposals of plugins integrations directly against Nagios monster project.
