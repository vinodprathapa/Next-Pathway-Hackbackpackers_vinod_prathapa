# Next-Pathway-Hackbackpackers_vinod_prathapa
Next Pathway Hackbackpackers problem statement resolutions
I can give the Lineage problem statement resolution
from the sql script which will be passed as input , get the originating table names 
search criteria as after the "from" and before next "space" as delimiter after the table name and one more condition is there should not be any brackets after "from"
so we can extract two table names with that search criteria

IDW_DATA.CNTRY_MULTI_DEF_CD_T
IDW_STAGE.CNTRY_MULTI_DEF_CD_S

now get the output columns fromt the sql query
search criteria:
text between SELECT and FROM --- one more condition is SELECT should not have any backets prior to it
then we get the column names as below

SWB_CNTRY_ID
CNTRY_TYPE_CD
DW_EFF_DT
DW_AS_OF_DT

INFORMATION_SCHEMA.COLUMNS
we can all the columns of a table in the database by executing a query that is " SELECT COLUMN_NAME FROM INFORMATION_SCHEMA.COLUMNS WHERE TABLE_NAME = '' "
we have to give the table names which we got at line 8 & 9 as input and we get the all column names.
then we can compare the column names from 16-19 lines in the above table column lists
then we can get the column name and corresponding originating table
