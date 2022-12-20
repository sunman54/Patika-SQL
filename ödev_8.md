## Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.<br />

#### 1- test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım .<br />

```SQL

CREATE TABLE employee (
  id SERIAL PRIMARY KEY,
  name VARCHAR(50) NOT NULL,
  email VARCHAR(100),
  birthday DATE
);

```

#### 2- Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.<br />

```SQL

insert into employee (name, email, birthday) values ('Pattin', 'pbuttle0@google.co.jp', '1983-05-22');
insert into employee (name, email, birthday) values ('Noni', 'nbrabben1@deliciousdays.com', '1987-08-24');
insert into employee (name, email, birthday) values ('Tris', 'trubega2@imgur.com', '1995-02-09');
insert into employee (name, email, birthday) values ('Georgina', 'gshepeard3@craigslist.org', '1984-03-24');
insert into employee (name, email, birthday) values ('Irvine', 'itew4@forbes.com', '1981-03-01');
insert into employee (name, email, birthday) values ('Pauly', 'poscannill5@skype.com', '1982-08-01');
insert into employee (name, email, birthday) values ('Jerrome', 'jmonkeman6@auda.org.au', '1984-06-25');
insert into employee (name, email, birthday) values ('Cathrine', 'cauten7@umich.edu', '1999-02-03');
insert into employee (name, email, birthday) values ('Valina', 'vaitken8@dyndns.org', '1983-09-20');
insert into employee (name, email, birthday) values ('Tilda', 'tfronczak9@cbslocal.com', '1997-02-16');
insert into employee (name, email, birthday) values ('Costa', 'cdemseya@zimbio.com', '1998-12-21');
insert into employee (name, email, birthday) values ('Persis', 'pjedraszczykb@technorati.com', '1985-10-30');
insert into employee (name, email, birthday) values ('Lusa', 'ltelferc@vk.com', '1994-10-22');
insert into employee (name, email, birthday) values ('Joannes', 'jorderd@squidoo.com', '1998-03-01');
insert into employee (name, email, birthday) values ('Bentley', 'bsherrarde@phoca.cz', '1985-01-15');
insert into employee (name, email, birthday) values ('Imojean', 'iedgeleyf@businesswire.com', '1999-08-13');
insert into employee (name, email, birthday) values ('Dorene', 'dwellardg@utexas.edu', '1985-07-15');
insert into employee (name, email, birthday) values ('Auberon', 'awenningtonh@yahoo.com', '1994-05-28');
insert into employee (name, email, birthday) values ('Lillis', 'lbentsoni@linkedin.com', '1994-02-08');
insert into employee (name, email, birthday) values ('Ernaline', 'enottramj@tumblr.com', '1982-05-12');
insert into employee (name, email, birthday) values ('Dorothee', 'descreetk@google.co.jp', '1998-07-25');
insert into employee (name, email, birthday) values ('Abby', 'adanilchenkol@1688.com', '1993-03-20');
insert into employee (name, email, birthday) values ('Cesya', 'cskinnm@goodreads.com', '1984-01-30');
insert into employee (name, email, birthday) values ('Lance', 'lgoggeyn@vimeo.com', '1984-03-16');
insert into employee (name, email, birthday) values ('Sisely', 'sabramskyo@admin.ch', '1993-11-10');
insert into employee (name, email, birthday) values ('Berti', 'banderp@qq.com', '1987-06-25');
insert into employee (name, email, birthday) values ('Cher', 'cfairsq@dagondesign.com', '1986-02-27');
insert into employee (name, email, birthday) values ('Garrek', 'gcollabiner@aol.com', '1983-07-22');
insert into employee (name, email, birthday) values ('Gustavus', 'godoghestys@walmart.com', '1981-07-06');
insert into employee (name, email, birthday) values ('Drugi', 'dcainest@nymag.com', '1986-07-03');
insert into employee (name, email, birthday) values ('Laural', 'lsigginu@squidoo.com', '1990-12-05');
insert into employee (name, email, birthday) values ('Brigit', 'bmarconev@dell.com', '1982-02-13');
insert into employee (name, email, birthday) values ('Tabbie', 'ttraskew@ameblo.jp', '1994-11-16');
insert into employee (name, email, birthday) values ('Quinn', 'qshetliffx@icio.us', '1981-11-18');
insert into employee (name, email, birthday) values ('Corny', 'cleggaty@google.it', '1990-07-17');
insert into employee (name, email, birthday) values ('Salomo', 'sduranz@twitpic.com', '1984-08-21');
insert into employee (name, email, birthday) values ('Karlene', 'kmacdougall10@theguardian.com', '1992-06-05');
insert into employee (name, email, birthday) values ('Grantley', 'gmoyles11@github.com', '1995-10-05');
insert into employee (name, email, birthday) values ('Abel', 'abellow12@sciencedirect.com', '1986-05-06');
insert into employee (name, email, birthday) values ('Rodie', 'rwelds13@dagondesign.com', '1983-04-01');
insert into employee (name, email, birthday) values ('Foss', 'fburk14@yolasite.com', '1990-01-21');
insert into employee (name, email, birthday) values ('Portia', 'pgoodbarr15@spiegel.de', '1998-01-31');
insert into employee (name, email, birthday) values ('Alick', 'agouge16@devhub.com', '1987-03-14');
insert into employee (name, email, birthday) values ('Hillie', 'hmackleden17@merriam-webster.com', '2000-12-01');
insert into employee (name, email, birthday) values ('Claire', 'cledingham18@jalbum.net', '1989-12-10');
insert into employee (name, email, birthday) values ('Torrey', 'tduggen19@list-manage.com', '1998-01-03');
insert into employee (name, email, birthday) values ('Leanora', 'lmoyle1a@theguardian.com', '1992-10-14');
insert into employee (name, email, birthday) values ('Rubin', 'rrenault1b@zimbio.com', '1984-12-14');
insert into employee (name, email, birthday) values ('Morgan', 'mpoytress1c@vistaprint.com', '1981-04-23');
insert into employee (name, email, birthday) values ('Farlee', 'fmiltonwhite1d@ft.com', '1998-10-22');

```


#### 3- Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.<br />

```SQL

SET name = 'kazım',
      email = 'kazım@gmail.com'
WHERE id = 3;


SET name = 'ragıp',
      email = 'ragıp@gmail.com'
WHERE id = 4;

SET name = 'avni',
      email = 'avni@gmail.com'
WHERE id = 5;

SET name = 'nazmi',
      email = 'nazmi@gmail.com'
WHERE id = 6;

```


#### 4- Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.<br />

```SQL

*DELETE FROM employee
WHERE id = 9;
*DELETE FROM employee
WHERE id = '31';
*DELETE FROM employee
WHERE id = 49;
*DELETE FROM employee
WHERE id = '13';

```
