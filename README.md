# MPI PDQ with Authentication

Example Apigee API Proxy to authenticate Patient Demographic Queries against the Master Patient Index (MPI).

The Patient Demographic Query (PDQ) API follows the [IHE specification](https://wiki.ihe.net/index.php/Patient_Demographics_Query).  It uses HL7 messages structures for the request and response. The `MSH.4/HD.1`  field in the message contains the ID of the **Assigning Authority**.

This API proxy checks that the sending application is authorised to send messages with that assigning authority.  The application must first be registered in the Apigee organisation and have been tagged with a custom attribute (AssigningAuthority) that contains the expected values of the `MSH.4/HD.1` segment.


//TODO: Add links to other Pre-requisites for set up TargetServers, Products etc.


