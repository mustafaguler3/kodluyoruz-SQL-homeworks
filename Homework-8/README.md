`~~1-Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
**CREATE TABLE employee (
  id SERIAL PRIMARY KEY,
  name VARCHAR(50) NOT NULL,
  email VARCHAR(100),
  birthday DATE
);**


2-Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.


**insert into employee (name, email, birthday) values ('Mack', 'mcartledge0@google.co.uk', '2008-07-22');
insert into employee (name, email, birthday) values ('Fredric', 'fweich1@com.com', null);
insert into employee (name, email, birthday) values ('Lanny', 'lklosser2@hc360.com', '2014-01-31');
insert into employee (name, email, birthday) values ('Gwenneth', 'gchesher3@jiathis.com', '2016-05-28');
insert into employee (name, email, birthday) values ('Lee', 'lgascone4@bloglovin.com', '2002-02-22');
insert into employee (name, email, birthday) values ('Wilton', 'wperello5@vimeo.com', '2003-05-27');
insert into employee (name, email, birthday) values ('Lusa', 'lmurden6@princeton.edu', '2019-09-27');
insert into employee (name, email, birthday) values ('Nariko', 'neakle7@bbc.co.uk', '2015-03-14');
insert into employee (name, email, birthday) values ('Tristan', 'tkrolik8@google.com.hk', '2015-07-27');
insert into employee (name, email, birthday) values ('Stephana', 'sjaukovic9@google.fr', '2015-01-08');
insert into employee (name, email, birthday) values ('Trever', 'tfaroa@1und1.de', '2006-05-18');
insert into employee (name, email, birthday) values ('Analise', null, '2016-10-23');
insert into employee (name, email, birthday) values ('Salim', 'swarrilowc@apache.org', '2001-11-28');
insert into employee (name, email, birthday) values ('Daryn', 'dcordinglyd@cbslocal.com', '2020-05-12');
insert into employee (name, email, birthday) values ('Irene', 'isherrye@miitbeian.gov.cn', null);
insert into employee (name, email, birthday) values ('Ethelda', 'eemanulssonf@reuters.com', '2019-09-05');
insert into employee (name, email, birthday) values ('Inglebert', 'ialsobrookg@nifty.com', '2008-02-11');
insert into employee (name, email, birthday) values ('Bradly', 'bkohlerh@networksolutions.com', '2013-06-12');
insert into employee (name, email, birthday) values ('Thurston', 'thandshearti@bigcartel.com', '2018-11-01');
insert into employee (name, email, birthday) values ('Gayelord', 'gpetrelloj@goodreads.com', null);
insert into employee (name, email, birthday) values ('Delaney', 'dedelheitk@answers.com', null);
insert into employee (name, email, birthday) values ('Domeniga', 'dhaselgrovel@jimdo.com', '2014-01-02');
insert into employee (name, email, birthday) values ('Garey', null, '2007-06-07');
insert into employee (name, email, birthday) values ('Jaye', 'jvonhagtn@diigo.com', '2018-07-31');
insert into employee (name, email, birthday) values ('Mort', 'millsleyo@reverbnation.com', null);
insert into employee (name, email, birthday) values ('Kellia', null, null);
insert into employee (name, email, birthday) values ('Edgard', 'epirazziq@smh.com.au', '2009-09-25');
insert into employee (name, email, birthday) values ('Juli', 'jferencr@statcounter.com', '2002-06-21');
insert into employee (name, email, birthday) values ('Ginger', 'gproscheks@amazon.co.uk', '2008-03-19');
insert into employee (name, email, birthday) values ('Morey', null, '2019-08-22');
insert into employee (name, email, birthday) values ('Holli', 'hobraddenu@bigcartel.com', null);
insert into employee (name, email, birthday) values ('Lew', null, '2007-08-21');
insert into employee (name, email, birthday) values ('Corbett', null, '2016-09-19');
insert into employee (name, email, birthday) values ('Egon', 'etredwellx@slideshare.net', '2016-10-04');
insert into employee (name, email, birthday) values ('Tadio', 'tnealeyy@google.cn', '2012-06-03');
insert into employee (name, email, birthday) values ('Shir', 'sleathartz@tiny.cc', '2012-06-03');
insert into employee (name, email, birthday) values ('Chryste', 'clindholm10@smugmug.com', '2007-10-31');
insert into employee (name, email, birthday) values ('Marrilee', 'mkynnd11@webmd.com', null);
insert into employee (name, email, birthday) values ('Greta', 'gvearnals12@hp.com', null);
insert into employee (name, email, birthday) values ('Karrie', 'kclapson13@mysql.com', '2014-10-12');
insert into employee (name, email, birthday) values ('Tanhya', 'timison14@merriam-webster.com', '2012-04-24');
insert into employee (name, email, birthday) values ('Erny', 'elemonby15@tmall.com', '2004-09-08');
insert into employee (name, email, birthday) values ('Cullin', 'cvillaret16@canalblog.com', '2011-07-01');
insert into employee (name, email, birthday) values ('Reynold', 'rmellem17@symantec.com', '2009-09-09');
insert into employee (name, email, birthday) values ('Mikol', 'mjachimiak18@taobao.com', '2005-02-11');
insert into employee (name, email, birthday) values ('Adolphus', null, '2013-06-02');
insert into employee (name, email, birthday) values ('Friederike', null, '2005-07-02');
insert into employee (name, email, birthday) values ('Lindy', 'lpetegrew1b@kickstarter.com', '2002-07-02');
insert into employee (name, email, birthday) values ('Normy', 'ngoathrop1c@shareasale.com', '2010-08-28');
insert into employee (name, email, birthday) values ('Elissa', 'eheninghem1d@engadget.com', null);**


3-Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

**UPDATE employee SET name = 'Ciguli', birthday = '24-06-2004' WHERE name = 'Elissa' RETURNING * ;
UPDATE employee SET  email = 'adana01@gmail.com' WHERE name = 'Ciguli' RETURNING * ;
UPDATE employee SET  email = 'adana01@gmail.com' WHERE name = 'Mack' RETURNING * ;
UPDATE employee SET  birthday = '24-06-2004' WHERE name = 'Mack' RETURNING * ;
UPDATE employee SET name = 'Ecrin', email = 'ecnebiecrin@gmail.com', birthday = '24-06-2004' WHERE name = 'Mack' RETURNING * ;**


4-Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

**DELETE FROM employee WHERE name = 'Fredric';
DELETE FROM employee WHERE id = 8;
DELETE FROM employee WHERE birthday = '2014-01-31';
DELETE FROM employee WHERE email = 'sjaukovic9@google.fr';
DELETE FROM employee WHERE name = 'F%';**~~`