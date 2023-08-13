# SqlServer-GenDDL
SqlServer script to generate DDL from command line. Not sure it works, saving for later.
 For more details see the original StackOverflow answer: 
 [https://stackoverflow.com/questions/6215459/t-sql-query-to-show-table-definition](https://stackoverflow.com/questions/6215459/t-sql-query-to-show-table-definition)

 Here are the details of that answer:

 Visit [http://www.stormrage.com/SQLStuff/sp_GetDDL_Latest.txt][1].

You will find the code of `sp_getddl` procedure for SQL Server.
The purpose of the procedure is script any table, temp table or object.

USAGE:

    exec sp_GetDDL GMACT

or

    exec sp_GetDDL 'bob.example'

or

    exec sp_GetDDL '[schemaname].[tablename]'

or

    exec sp_GetDDL #temp

I tested it on SQL Server 2012, and it does an excellent job.

I'm not the author of the procedure.  Any improvement you make to it send to Lowell Izaguirre (scripts@stormrage.com).


  [1]: http://www.stormrage.com/SQLStuff/sp_GetDDL_Latest.txt
