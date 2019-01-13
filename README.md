# Net IT Web dev project - 2018
## DataBase setup
CREATE USER 'wd_2018u'@'localhost' IDENTIFIED VIA mysql_native_password USING '***';<br>
GRANT USAGE ON . TO 'wd_2018u'@'localhost' REQUIRE NONE WITH MAX_QUERIES_PER_HOUR 0 MAX_CONNECTIONS_PER_HOUR 0 MAX_UPDATES_PER_HOUR 0 MAX_USER_CONNECTIONS 0<br>
GRANT SELECT, INSERT, UPDATE, DELETE ON wd\_2018.* TO 'wd_2018u'@'localhost';

### `user` - User table
- user id

CREATE TABLE wd_2018.user ( user_id INT NOT NULL AUTO_INCREMENT , email VARCHAR(50) NOT NULL , password VARCHAR(64) NOT NULL , rights INT NOT NULL DEFAULT '0' , active INT NOT NULL DEFAULT '0' , PRIMARY KEY (user_id)) ENGINE = InnoDB;

- emeil
- password
- rights
- active

### `page` - Pages table
- page_id
- cat_id
- lang_id
- uri
- html_title
- html_description
- html_keywords
- heading
- content
- active

### `menu` - Menus table
- manu_id
- manu_text
- lang_id
- iri
- cat_id
- position
- activ

### `lang` - Language
- lang_id
- slug
- name
- active
### `cat`- Categories table
- cat_id
- lang_id
- name
- active

## PHP Boilerplate

### Routing
- .htaccess setup
- Get base folder
- Get URI
- AutoLoader
- MVC?

Example:<br> **address1/address2**(C:default,A:deafult)<br>
**admin/page_edit**(C:admin,action:page_edit)<br>
**ajax/page_name**(C:ajax,action:page_name)
### Templete sisteme
### DataBase management

## Project high level
TODO!!! - $title and $description functionalization

### Tamplete
### Base Functionalities
### Admin part
- Login
- Menus
- Pages

#### Login
#### Menus
#### Pages

### Backend API (Services)
## Mobile application

