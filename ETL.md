## ETL components

### Design for Failure

- Check the connection;
- Ping host;
- Row count condition;
- Check the folder for file exists;
- Check if table or column exists;
- Timeoout for FTP, API, SSH
- Connection retry;
- Independent components;
- version control

### Change Data Capture
Use the Updated_timestamp to track the CDC.


### Data Profiling

- How many NULL or empty values in a column \ table;
- Check DISTINCT values;
- MIN/MAX/AVG values;
- MIN/MAX/AVG string length;
- Patterns (date, phone numbers, etc.);
- Data Distribution;

### Data Validation \ Data testing
- Unit testing after ETL job completes;


### ETL requirements
1. Connectivity - the tool should be able to connect to DB adn read different file formats;
2. Platform independence - Windows/Linux;
3. Scalability - parallel workflows, claster;
4. Design  Flexibility/Reuse - should be easy to make transformations and create/copy new workflows;
5. Extensibility - can we create a new functionality?
6. Security (Authorisation\Authentification) - roles distinguishing;
7. Admin;
8. Version Control/Change Requests;
9. Disaster Recovery/Backup;
10. Infrastructure as as Code - for clouds mostly or self-written tools;
11. 3rd party integration - integration with email or other services;
12. Opportunity to use programming languages


### Data Transformations
- Slowly Change Dimensions (Dimensional Modelling);
- Lookup;
- Pivot/Unpivot;
- Parameters;
- Loops;
- Aggregations;
- Creating new columns;
- sorting, joins, unions

### Testing and Debugging

### Lineage and Impact Analysis
can we track the whole line from source to the target?

### Logging and Auditing
- better to log etl to DB
- better create a dashboard for users based on logs 