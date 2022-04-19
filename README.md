# SQL CHEAT

### Create & use DATABASE
``` CREATE DATABASE nom_de_la_bdd;```<br>
``` USE nom_de_la_bdd; ```

#### List all Databases 
```SHOW DATABASES;```

#### Delete Database 
```DROP DATABASE nom_de_la_bdd;```

### TABLES 

#### Create table
```
CREATE TABLE nom_de_la_table (
    id INT PRIMARY KEY AUTO_INCREMENT NOT NULL,
    name VARCHAR(150) NOT NULL,
    age INT NOT NULL,
    is_visible BOOL NULL,
    address TEXT NULL,
    birthday DATE NULL
);
```
#### Display structure table
```DESCRIBE nom_de_la_table;```

#### Display values from table
```SELECT * FROM nom_de_la_table;```

#### List all Tables 
```SHOW TABLES;```

#### Insert value(s) 
```INSERT INTO nom_de_la_table (name, age, is_visible, address, birthday) VALUES ('plop', 15, 1, 'la fayette 75010', '1985-01-01'), (Other values) , (Other values);```

#### Change structure of table
``` ALTER TABLE nom_de_la_table ADD nom_colomn TYPE OPTION;```<br>
Exemple pour ajouter une colonne : <br>
``` ALTER TABLE nom_de_la_table ADD zipcode INT NOT NULL;```

#### Update value
``` UPDATE nom_de_la_table SET nom_colomn='value';``` <br>
``` UPDATE nom_de_la_table SET nom_colomn='value' WHERE id=1;```

#### Delete value
``` DELETE FROM nom_de_la_table WHERE *condition*;```<br>
``` DELETE FROM nom_de_la_table WHERE id=1;```

#### Delete all values from table
``` TRUNCATE TABLE nom_de_la_table;```

#### Delete table
``` DROP TABLE nom_de_la_table;```
