# databaserepo
CREATE TABLE user
(
id int(11),
LastName varchar(255),
FirstName varchar(255),
Address varchar(255),
age int
);

CREATE TABLE user_account_type
(
id int(11),
 account_type varchar(255),
date varchar(255),
garrantor_name varchar(255),
naxt-of-kin varchar(255)
);

CREATE TABLE transactions
(
id int(11),
current_balance int(1000),
previous_balance int(10000),
last_withdrawer int(100),
last_deposit int(10000)
);




INSERT INTO user (firstname,lastname,age,address) 
	VALUES ("Ede", "obinna", 27, "12 chezoka estate" );

INSERT INTO user_account_type (account_type,date,garrantor_name,next-of-kin)
	VALUES("savings","12 july 2016","Tony","bola");

INSERT INTO transactions (current_balance,previous_balance,last_withdrawer,last_deposit)
	VALUES(100000,200000,12000,10000);

SELECT * FROM user WHERE id = 19862;

SELECT id,firstname,lastname FROM user WHERE lastname = "obinna";

SELECT count(id) FROM user WHERE firstname = "obinna";

DELETE FROM user WHERE id = 53637 AND id = 53425 LIMIT 1;

SELECT COUNT(id) as person FROM user WHERE firstname LIKE "firstname%";





