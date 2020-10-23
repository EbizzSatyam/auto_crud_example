# what is this
this package to create auto crud operation in node js
# mysql-crud-node Installation
`npm install --save mysql-crud-node`

Then...

...
import {mysqlCrudNode} from `mysql-crud-node`;

mysqlCrudNode({
    table_name:'users',
    table_fields:{
        name:STRING,
        emal:STRING,
        password:TEXT
        },
    valid_fields:{
        name:{required,min:2}
        email:{email,required}
        password:{min:6}
    }
});
...

## Options

In this package 3 Optionans are there

* *table_name* here is your table name 
* *table_fields* here is your table fields name list
* *valid_fields* here is your table fields multiple vaidation list / (default to false)

