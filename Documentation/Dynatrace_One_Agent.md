# Dynatrace OneAgent	

## Overview

This bundle of advanced actions allows you to take advantage of the integration between NeoLoad and Dynatrace OneAgent. 
This bundle has the following actions:
* DynatraceEvents   
  Links a load testing event to all services used by an Application monitored by Dynatrace
* DynatraceMonitoring   
    * Retrieve Infrastructure and Services metrics from DynaTrace and insert them in NeoLoad External Datas so that
      you can correlate NeoLoad and DynaTrace metrics within NeoLoad.
    * Send the global statistics of the test to Dynatrace OneAgent so that it can be used as custom metrics 
      in Dynatrace dashboards.
      
     
| Property | Value |
| -----| -------------- |
| Version  | 1.0.0 |
| Maturity | Experimental |
| Author   | Neotys Partner Team |
| License  | [BSD Simplified](https://www.neotys.com/documents/legal/bsd-neotys.txt) |
| NeoLoad  | 6.1 (Enterprise or Professional Edition w/ Integration & Advanced Usage and NeoLoad Web option required)|
| Requirements | NeoLoad Web SaaS subscription |
| Bundled in NeoLoad | No
| Download | See [latest release](https://)


## Set-up

1. Create a User Path “Dynatrace”
1. Insert DynatraceEvents in the ‘End’ block.
1. Insert DynatraceMonitoring in the ‘Actions’ block.
1. Create a Population “Dynatrace” that contains 100% of User Path “Dynatrace”
1. In the Runtime section, select your scenario, select the “Dynatrace” population and define a constant load of 1 user.

## Parameters for Dynatrace Events

| Name             | Value |
| -----            | ----- |
| Dynatrace_ID     |  Id of your saas dynatrace environment (http://<id>.live.dynatrace.com) |
| Dynatrace_API_KEY| API key of your dynatrace account |
| Tags (optional)  | Dynatrace Tags of the services used by your SUT |
| EventStatus      |: status sent to dynatrace : START or STOP |
| Dynatrace_Managed_Hostname (Optional) | Hostname of your dynatrace managed environment |


