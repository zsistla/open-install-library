# Error Codes

The following page list all the various error codes the newrelic-cli(install) can return,
Please note, some error code values may be generated by other downstream processes. For example, an error code value of 1 may be generated through various executions. It can be generated because an On-Host Integration noticed the infra structure agent is not installed. But that value could also be generated when starting up the infrastructure agent un-successfully.

| Error Code | Recipe | Error Message|
|-----|----|----|
| 1  | infrastructure-agent-installer | The infrastructure agent was not detected but is required in order to install an On-Host Integration |
| 2  | infrastructure-agent-installer | An OHI is failing when validating the provided input can connect to a 3rd party software. This can be an nginx  apache status route, or a user login/password permission for a database
| 2  | mongodb-open-source-integration | Cannot connect to the server |
| 3  | apm | No processes found to monitor|
| 3  | mongodb-open-source-integration | Cannot connect to the server using the provided username/password and hostname/port |
| 5  | dotnet-agent-installer | IIS is not installed |
| 6  | dotnet-agent-installer | ASP.NET is not installed |
| 7  | dotnet-agent-installer | Insufficient permissions |
| 9  | elasticsearch-open-source-integration | The ElasticSearch config file cannot be found |
| 10 |  | For linux, `grep` is not installed and required to install |
| 11 | elasticsearch-open-source-integration | SSL is set to true, but CA bundle directory cannot be found |
| 11 | mongodb-open-source-integration | SSL is set to true, but client certificate file cannot be found |
| 11 |  | For linux, `sed` is not installed and required to install |
| 12 |  | For linux, `awk` is not installed and required to install |
| 12 | elasticsearch-open-source-integration | SSL is set to true, but CA bundle file cannot be found |
| 13 | mongodb-open-source-integration | SSL is set to true, but CA file cannot be found |
| 13 |  | For linux, `cat` is not installed and required to install |
| 14 |  | For linux, `tee` is not installed and required to install |
| 15 |  | For linux, `touch` is not installed and required to install |
| 18 |  | Attempt to install within a docker container. The user should instead run the install on the host, not in the container |
| 19 |  | Attempt to install within a Microsoft Subsytem Linux container. This is not supported |
| 20 |  | For linux, systemctl is not available on the host (either nor present or not running) |
| 21 |  | There is no newrelic infrastructure agent available for the host |
| 22 |  | Recipe depedency not met |
| 23 |  | User declined to accept recipe terms |
| 130 | | Installation was cancelled either using Ctrl+C or by selecting not to continue the installation |